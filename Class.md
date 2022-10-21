## Class
# Немного по этой теме
**Python** имеет множество встроенных типов, например, `int`, `str` и так далее, которые мы можем использовать в программе. Но также Python позволяет определять собственные типы с помощью классов. Класс представляет некоторую сущность. Конкретным воплощением класса является объект.
*Можно еще провести следующую аналогию.* У нас у всех есть некоторое представление о человеке, у которого есть имя, возраст, какие-то другие характеристики Человек может выполнять некоторые действия - ходить, бегать, думать и т.д. То есть это представление, которое включает набор характеристик и действий, можно назвать классом. Конкретное воплощение этого шаблона может отличаться, например, одни люди имеют одно имя, другие - другое имя. И реально существующий человек будет представлять объект этого класса.
Класс определяется с помощью ключевого слова `class`:

![Картина](/image2.png.jpg)

```Python
class Human:
    def __init__(self, name):
        self.name = name
        self.children = []

    def add_child(self, child):
        if child is not self:
            self.children.append(child)

    def add_child(self, child):
        self.child = child
    def add_father(self, father):
        self.father = father
    def add_mother(self, mother):
        self.mother = mother
vasya = Human("Вася")
oleg = Human("Олег")
dasha = Human("Dasha")
oleg.add_father(vasya)
vasya.add_child(oleg)
oleg.add_mother(dasha)
print(vasya.child.name)
print(oleg.father.name)
print(oleg.mother.name)


