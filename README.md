# iOS
cour iOS

http://swiftlang.ng.bluemix.net/#/repl/5821b7cbbe1f3f272165e091


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
