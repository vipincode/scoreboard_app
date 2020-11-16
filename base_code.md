import React from 'react';
import ReactDOM from 'react-dom';

// CREATING HEADER COMPONENT

const Header = () =>
  <header>
    <h1>Scorboard</h1>
    <span className="stats">Player: 1</span>
  </header>

// CREATING PLAYER COMPONENT

const Player = () => {
  return(
    <div className="player">
      <span className="player-name">
        vipin
      </span>
      {/*Compostion method in React*/}
      <Counter />

    </div>
  );
}

// CREATING COUNTER COMPONENT

const Counter = () => {
  return(
    <div className="counter">
      <button className="counter-action decrement">-</button>
      <span className="counter-score">35</span>
      <button className="counter-action increment">+</button>
    </div>
  );
}

const App = () => {
  return(
    <div className="scoreboard">
      <Header />

      {/*Player Counetr*/}
      <Player />
    </div>
  );
}

ReactDOM.render(
    <App />,
    document.getElementById('root')
);














