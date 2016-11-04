# iOS
cour iOS

https://swiftlang.ng.bluemix.net/#/repl/581c7531b2e9b157d8c9b89b


//Challenge A
//Repeat a task
// x fois
func result() {
    print("Hello World")
}
func repeatTask(times y: Int, task: () -> Void){
    for i in 1...y {
        task()
    }
    
    }
    
repeatTask(times : 10, task : result);

// Challenge B
// Repeat operations x fois
// operation take the current itération
// return the sum of all itération operations
// Start iterations from 1 to times

func mathSum(times x: Int, operation: (Int) -> Int) -> Int {
    
    var result = 0
    
    for i in 1...x {
        result += operation(i)
    }
    
    return result
}

mathSum(times: 10, operation: fibonacci)
