# Python-5
# Activity 1
class mobilephone:
    def __init__(self, brand, model, os_version):
        self.brand = brand
        self.model = model
        self.os_version = os_version
    def power_on(self):
        return f"{self.brand} {self.model} uses {self.os_version} to operate!"

class smartphone(mobilephone):
    def __init__(self, brand, model, os_version):
        super().__init__(brand, model, os_version)
    def power_on(self):
        return f"{self.brand} {self.model} uses {self.os_version} to operate!"

        
phone1 = mobilephone("Nokia", "Asha", "Series40" )
phone2 = smartphone("Samsung", "S20", "Android 13" )

print(phone1.power_on())
print(phone2.power_on())

# Activity 2
class Lion:
    def move(self):
        return "walk"

class Snake:
    def move(self):
        return "slither"

class Eagle:
    def move(self):
        return "fly"

for animal in [Lion(), Snake(), Eagle()]:
    print(animal.move())
