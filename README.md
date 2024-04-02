# cubs
class Cuboid:
    def __init__(self, length, width, height):
        self.length = length
        self.width = width
        self.height = height

    def volume(self):
        return self.length * self.width * self.height

    def surface_area(self):
        return 2 * (self.length * self.width + self.length * self.height + self.width * self.height)


def main():
    length = float(input("Enter the length of the cuboid: "))
    width = float(input("Enter the width of the cuboid: "))
    height = float(input("Enter the height of the cuboid: "))

    cuboid = Cuboid(length, width, height)

    print("Volume of the cuboid:", cuboid.volume())
    print("Surface area of the cuboid:", cuboid.surface_area())


if __name__ == "__main__":
    main()
