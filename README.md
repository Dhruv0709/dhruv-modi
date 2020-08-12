class Deque:
    def _init_ (self) :
        self. data = []

    def is_empty(self):
        if len(self.data) == 0:
            return 0
        else:
            return 1

    def add_first(self, value):
        self.data.insert(0, value)
        print(self.data, 'first element added')
        
    def add_last(self, value) :
        self.data.append(value)
        print(self.data, 'last element added')

    def del_first(self):
        if self.is_empty() == 1:
            print('first element deleted which is', self.data.pop(0))
            print(self.data)
        else:
            print('The stack is empty')

    def del_last(self):
        if self.is_empty() == 1 :
            print('last element deleted which is', self.data.pop(0))
            print('self.data')
        else:
            print(' Stack is empty')

d = Deque()
d.add_first(2)
d.add_first(1)
d.add_first(3)
d.add_first(4)
d.del_first()
d.del_last()
