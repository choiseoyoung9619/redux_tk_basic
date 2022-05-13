# Project 설명

`npx create-react-app ts-react-reduxtk --template redux-typescript` 로 만들어진 자료  
기본적으로 Counter.tsx 컴포넌트가 구현되어 있어서 "reduxTK"의 basic한 구조를 확인할 수 있다  
([참고한 링크](https://blog.logrocket.com/using-typescript-with-redux-toolkit/))

### ReduxTK 구조

**index.tsx** : Provider store={store} 설정  
**App.tsx**  
**Counter.tsx**  

**CounterSlice.ts**  
createSlice를 통해 initialState, reducers, extraReducers를 정의한 action 생성  
createAsyncThunk(reduxTK 내장 미들웨어)를 통해 비동기 처리 (axios 등등)  
생성한 action을 export해서 Counter.tsx컴포넌트에서 useSelector, useDispatch를 통해 state에 접근, action을 수행  

* Reducer 란 ? 현재state와 action객체를 파라미터로 받아와서새로운 state를 반환해주는 함수   
`const [state, dispatch] = useReducer(reducer, initialState);`

----
`npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.


