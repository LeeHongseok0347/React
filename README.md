# React 
리액트는 nodejs서버 상에서 동작하는 프론트엔드 작성용 라이브러리다.
## 기본 동작 원리

1. index.html하나로 단일페이지로 실행되며, 바디부분에서 변화가 일어난다.  
2. index.js 파일에서 다른 js파일들을 변수로 매핑해준다.
3. index.html에서 변수로 매핑된 js파일을 바디부분에 넣어준다.  


    //App.js  : App를 정의한다.
    function App() {
      return <div> hello </div>
    }
    export default App;
      
    //index.js : App를 root라는 이름으로 매핑해준다.
    const root = ReactDOM.createRoot(document.getElementById('root'));
    root.render(<App />);
    
    //index.html : root를 표시해 준다.
    <body>
      <div id="root"></div>
    </body>
    
    
## 기본 동작 원리

