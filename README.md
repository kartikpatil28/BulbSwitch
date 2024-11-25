# Bulb Switch Project

This project is a simple React application demonstrating a light bulb switch feature. The application allows users to toggle a bulb on and off, changing its appearance and shadow dynamically.

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Components](#components)
- [Styling](#styling)
- [License](#license)

## Introduction
The Bulb Switch Project is a basic React application created to demonstrate state management, conditional rendering, and dynamic styling using Tailwind CSS. Users can interact with a button to turn a bulb on and off.

## Features
- Toggle a bulb on and off with a button click
- Dynamic styling using Tailwind CSS
- Responsive design

## Installation
To get started with this project, clone the repository and install the necessary dependencies.


```bash
git clone https://github.com/kartikpatil28/BulbSwitch.git
cd BulbSwitch
npm install

```

## Usage
I have included the setup.md file on how to run the project in your local machine. Please read it carefully and if you find any difficulty or a bug please reac out to me on my linkedin or twitter account. 
If you have great ideas/ suggestions please do raise an issue.

## Components

```
import React, { useState } from "react";

const Bulb = () => {
  const [isOn, setIsOn] = useState(false);

  const toggleBulb = () => {
    setIsOn(!isOn);
  };

  return (
    <div className="bg-black min-h-screen flex flex-col justify-center items-center">
      <h1 className="font-extrabold text-4xl mb-8 text-purple-700">
        BULB SWITCH
      </h1>
      <div className="flex items-center">
        <button
          className="p-3 text-white bg-blue-500 rounded-lg shadow-lg mr-4 hover:bg-blue-600 transition duration-300"
          onClick={toggleBulb}
        >
          ON/OFF
        </button>
        <div
          onClick={toggleBulb}
          className={`w-[150px] h-[150px] rounded-full ${isOn ? 'bg-yellow-400 shadow-[0_0_40px_yellow] transition-all duration-300' : 'bg-black'}`}
        ></div>
      </div>
    </div>
  );


};

export default Bulb;

```
## Styling
For styling i have used Tailwind CSS for major part of this project. I have taken some improvement suggestions from the AI tools like ChatGPT and Microsoft Copilot to improve the UI.


## License
MIT License

Copyright (c) 2024 Kartik

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
