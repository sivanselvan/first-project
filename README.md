<html>
<header><title>This is title</title></header>
<body>
  <h1>Hello world</h1>
  <h1>This is a website which supports the LGBTQ community</h1>
  import React, { useCallback, useState } from 'react';
import Button from '@material-ui/core/Button';
import logo from './logo.svg';
import './App.css';

function App() {
  const [picOn, setPicOn] = useState(false);
  const switchPicOn = () => {
    setPicOn(!picOn);
  };
  return (
    <div className='App'>
      <header className='App-header'>
        <p>
          {picOn ? (
            <img
              alt="sivan.selvan's profile pic"
              class='_6q-tv'
              src='https://instagram.fmaa1-1.fna.fbcdn.net/v/t51.2885-19/s150x150/80403356_777162789418188_3604942166666772480_n.jpg?_nc_ht=instagram.fmaa1-1.fna.fbcdn.net&amp;_nc_ohc=WgJA1Xtev6UAX-MUS02&amp;oh=d08285cf32796ea34a435a166fc7253e&amp;oe=5EAE5A71'
            />
          ) : null}
          <br />
          <Button variant='contained' color='primary' onClick={switchPicOn}>
            SIVAN SELVAN (CLICK TO {picOn ? 'HIDE' : 'SEE'} BEAUTY)
          </Button>
        </p>
      </header>
    </div>
  );
}

export default App;
</body>
</html>
