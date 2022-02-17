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

```

## class 03

Create state in App, that can be passed as a propertie to header(number of hearts)

need to create function in App.js to handle changing app state


build a constructor

```js
constructor(props){
    super(props);
    this.state = {
      hearts: ''
    }
}

// create method

  addHearts= () => {
    this.setState({
      hearts: this.state.hearts + 'emoji'
    })
  }

render(){
    return(
      <Header hearts={this.state.hearts} />
      <header>
        <h1>Hello World</h1>
      </header>
    );
  }
}

// access props in header

 render(){ // must have
    return ( // must have
      <>  // one parent element use a fragment
      <header>
        <HeaderHello World {this.props.hearts}>
        // access method 
      <Main data={data} addHearts ={this.addHearts}


send props to horned beast

<hornedBeast
  addHearts={this.props.addHearts}>


  // add onclick to image

  onclick={this.props.addHearts}
```

setting up a modal
should live in app.js and so should the state
```js



```