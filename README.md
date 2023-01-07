# Initializers



**Initializers**
```
struct InitializerStruct {
    var initializerProperty: String
}
var initializerObject = InitializerStruct(initializerProperty: "Ahmet") //memberwise initializing and "Ahmet" is a default property


struct InitializerStruct2 {
    var property: String
    init() {    //custom initializer
        property = "Ahmet"
        print("Creating a new initializer")
    }
}
var initializerObject2 = InitializerStruct2() // property = "Ahmet"
initializerObject2.property = "Ali"


struct InitializerStruct3 {
    var property1: String
    var property2 = 0 // default value 
}
let initializerObject3 = InitializerStruct3(property1: "Alex")
let initializerObject4 = InitializerStruct3(property1: "Ahmet", property2: 23)


struct InitializerStruct4 {
    var property: String
    var property2 = 0
    
    init() {
        self.property = "Ahmet"
        print("Creating a string name \(property)")
    }
}
let initializerObject5 = InitializerStruct4()

struct InitializerStruct5 {
    var property: String
    var property2 = 0
}

extension InitializerStruct5 {
    init() {
        self.property = "Ahmet"
    }
}
let initializerObject6 = InitializerStruct5(property: "Ali")
let initializerObject7 = InitializerStruct5()
```

