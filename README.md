x = "global"

def outer():
    x = "enclosing"
    
    def inner():
        x = "local"
        print("Inner x:", x)
    
    inner()
    print("Outer x:", x)

outer()
print("Global x:", x)
