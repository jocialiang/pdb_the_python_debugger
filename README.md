# pdb_the_python_debugger
a short notes of pdb, it will be useful when you are implementing your model with an unfriendly framework such as Mxnet.
## log_in.py  
    class User():
      def __init__(self, name):
          self.name = name
          self.password = 'hello world'
      def log_in(self, password):
          if password == self.password:
              print('login success')
          else:
              print('your password is not correct')
  
      if __name__ == '__main__':
        user = User('Mike')
        user.log_in('abcd')
        user.log_in('hello world')
## Command
    l, list line
    l n, list from line n
    b n, set breaking point at line n
    c, execute
    n, execute next line
    p variable, print variables
    s, step in function
    q, quit debugging mode
## Run pdb
python -m pdb log_in.py
## Results
![Alt text](https://github.com/jocialiang/pdb_the_python_debugger/blob/master/pdb_1.jpg)
![Alt text](https://github.com/jocialiang/pdb_the_python_debugger/blob/master/pdb_2.jpg)
![Alt text](https://github.com/jocialiang/pdb_the_python_debugger/blob/master/pdb_3.jpg)
