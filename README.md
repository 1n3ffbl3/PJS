Version 2 Function

1. 

makeTurkeySandwich 
	Get one slice of bread.
	Add  turkey.
	Put a slice of bread on top.

function makeTurkeySandwich (){
	Get one slice of bread;
	Add  turkey;
	Put a slice of bread on top;
}
makeTurkeySandwich()

2. Customizing functions 

function makeSandwichWith (filling){
	Get one slice of bread;
	Add  filling;
	Put a slice of bread on top;
}
makeSandwichWith()
e.i. makeSandwichWith(ham)

// console.log(makeSandwichWith(ham))

3. More on customizing functions

function sayHiTo(person){
	console.log('hi', person);
}

4. It should have a function to display todos

var todos = ['item 1', 'item 2', 'item 3'] 

function displayTodos(){
	console.log("My todos:", todos);	
}

displayTodos()

5. It should have a function to add todos

function addTodos(todo){
	todos.push(todo);
	displayTodos();
}


6. It should have a function to change todos

function changeTodo(position, newValue){
	todos[position] = 'newValue';
	displayTodos();
}

changeTodo(0, 'changed')

7. It should have a function to delete todos

function deleteTodo(position){
	todos.splice(position, 1);
	displayTodos();
}

8. Observations

var myName="Gordon";

function sayName(){
	console.log(myName);
}

//If you're inside of a function, you can look out and see data, but the opposite isn't true. If you're outside, you can't look in.

9. Circles and arrows



