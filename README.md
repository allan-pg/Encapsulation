# Encapsulation
Encapsulation is just enclosing your data to prevent contents from being changed.
class Car:
	__maxspeed = 0
	__name = ''
	def __init__(self):
		self.__maxspeed = 400
		self.__name = 'Ferrari'
	def drive(self):
		print('Your', self.__name, 'is starting')
		print(self.__maxspeed)
	def setspeed(self, speed):
		self.__maxspeed = speed
class Sportcar(Car):
	pass
car = Car()
car.setspeed(350)
print(car.drive()) #You can only change the speed by accessing set speed method 
