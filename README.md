# LA-26

FILE NAME - turle.py
from abc import ABC, abstractmethod
class NinjaTurtle(ABC):
    @property
    @abstractmethod
    def alias(self):
        pass
    
class Leonardo(NinjaTurtle):
    def  __init__(self, real_name, alias):
        self.real_name = real_name
        self.__alias = alias
    
    @property
    def alias(self):
        return f"{self.__alias}"

class Michelangelo(NinjaTurtle):
    def  __init__(self, real_name, alias):
        self.real_name = real_name
        self.__alias = alias
    
    @property
    def alias(self):
        return f"{self.__alias}"

class Donatello(NinjaTurtle):
    def  __init__(self, real_name, alias):
        self.real_name = real_name
        self.__alias = alias
    
    @property
    def alias(self):
        return f"{self.__alias}"

class Raphael(NinjaTurtle):
    def  __init__(self, real_name, alias):
        self.real_name = real_name
        self.__alias = alias
    
    @property
    def alias(self):
        return f"{self.__alias}"

-main.py
FILE NAME - LA#26
import turtle

leo = turtle.Leonardo("Leonardo","Katana")
gelo = turtle.Michelangelo("Michelangelo","Nunchakaku")
tel = turtle.Donatello("Donatello","Boxstaff")
rap = turtle.Raphael("Raphael","Sai")

print(leo.alias)
print(gelo.alias)
print(tel.alias)
print(rap.alias)
