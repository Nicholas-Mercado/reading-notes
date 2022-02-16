# Lecture notes c301

## Class 01

### Create a React app

remove app.test, logo, reportWEb, Setup test
call it Gallery-of-Horns repo
```js
import React from 'react';

class App extends React.Component {
  render(){ // must have
    return ( // must have
      <>  // one parent element use a fragment
      <header>
        <h1>Hello World</h1>
      </header>
      <main>
        <Person name="Nick"/> // importing component
        <Person name="CHRIS"/> // importing component
        <Person name="jim"/> // importing component
        <Person name="Eric"/> // importing component
        // <article>
        //   <h3>ME</h3>
        //   <p>
        //     lorem fsadkifndsaokgnakognakognakognkoangkopang
        //   </p>
        // </article> // use this to create a compoinet
      </main>
      <footer>
      </footer>
      </>
    );
  }
}
export default App;

create a file for each Main.js
Header.js
class Header extends React.Component{
  render(){
    return(
      <Header />
      <header>
        <h1>Hello World</h1>
      </header>
    );
  }
}

export default App;


Person.js // component 

import React from 'react';

class Person extends React.Component{
  render(){
    return(
      <article>
          <h3>{this.props.name}</h3>
          <p>
            lorem fsadkifndsaokgnakognakognakognkoangkopang
          </p>
        </article>

    )
  }
}

export default Person;
