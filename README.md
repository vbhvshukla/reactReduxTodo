Steps :
1) Start by creating a store (single source of store)
2) In store we have configureStore function
3) we must give reducer in configureStore
4) Now we built todoSlice which is created by createSlice which has name,initial state and reducers(also called functins).
5) In initial state we built a todos object which contains id and todo message.
6) Reducers are objects in which we can give key : value(functions) pairs
7) In reducers we get access of two things state and action
8) In state we get the current state in the store.
9) In action we get action.payload (text)
10) We can update the state by state.todos.push(todo)
11) Now we must export every individual reducer separately and export the main source reducer as well todoSlice.reducer
12) In components , we must dispatch a value by useDispatch(addTodo(input)) to the store.
13) in Todos.js component we must select the state from the store by using useSelector(state=>state.todos)