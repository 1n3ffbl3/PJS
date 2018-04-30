README.md

var myComputer = {
	operatingSystem: "mac",
	screenSize: "15 inches",
	purchaseYear: 2011
};

myComputer.operatingSystem // "mac"

2. Objects and functions 

var gordon = {
	name: "Gordon";
	sayName: function(){
		console.log(this.name); //"this" will refer to that object
	}
}

gordon.sayName();

3. It should store the todos array on an object

var todoList = {
	todos:['item 1, 'item 2', 'item 3']
};

4. It should have a displayTodos method

var todoList = {
	todos:['item 1, 'item 2', 'item 3'],
	displayTodos: function(){
		console.log('My Todos', this.todos);
	}
};

5. It should have an addTodo method

var todoList = {
	todos:['item 1, 'item 2', 'item 3'],
	displayTodos: function(){
		console.log('My Todos', this.todos);
	},
	addTodo: function(todo){
	this.todos.push(todo);
	this.displayTodos();
	}
};


6. It should have a changeTodo method

var todoList = {
	todos:['item 1, 'item 2', 'item 3'],
	displayTodos: function(){
		console.log('My Todos', this.todos);
	},
	addTodo: function(todo){
	this.todos.push(todo);
	this.displayTodos();
	},
	changeTodo: function(position, newValue){
	this.todos[position] = newValue;
	this.displayTodos();
	}
};

7. It should have a deleteTodo method


var todoList = {
	todos:['item 1, 'item 2', 'item 3'],
	displayTodos: function(){
		console.log('My Todos', this.todos);
	},
	addTodo: function(todo){
		this.todos.push(todo);
		this.displayTodos();
	},
	changeTodo: function(position, newValue){
		this.todos[position] = newValue;
		this.displayTodos();
	},
	deleteTodo: function(position){
		this.todos.splice(position,1);
		this.displayTodos();
	}
};