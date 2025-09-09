/* Reset & base */
* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

body {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  background-color: #1B2A41; /* default background */
  color: #e0e6f0;
  transition: background-color 0.8s ease;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 20px;
}

.container {
  background: rgba(255, 255, 255, 0.05);
  border-radius: 12px;
  max-width: 700px;
  width: 100%;
  padding: 30px 40px;
  box-shadow: 0 8px 20px rgba(0,0,0,0.3);
  backdrop-filter: blur(10px);
}

header {
  text-align: center;
  margin-bottom: 30px;
}

header h1 {
  font-size: 2.4rem;
  margin-bottom: 8px;
  color: #f0f4f8;
  text-shadow: 0 2px 6px rgba(0,0,0,0.5);
}

header p {
  font-style: italic;
  color: #aab8d3;
  font-size: 1.1rem;
}

.slider {
  position: relative;
  overflow: hidden;
  min-height: 220px;
}

.slides {
  position: relative;
}

.slide {
  position: absolute;
  top: 0; left: 0;
  width: 100%;
  opacity: 0;
  transform: scale(0.95);
  transition: opacity 0.8s ease, transform 0.8s ease;
  color: #e0e6f0;
  padding: 10px 5px;
  pointer-events: none;
}

.slide.active {
  opacity: 1;
  transform: scale(1);
  position: relative;
  pointer-events: auto;
}

.slide h2 {
  color: #a3c4f3;
  margin-bottom: 15px;
  font-weight: 600;
  text-shadow: 0 1px 3px rgba(0,0,0,0.4);
}

.slide p, .slide ul {
  font-size: 1.1rem;
  line-height: 1.5;
  color: #d0d8e8;
}

.slide ul {
  list-style-type: disc;
  padding-left: 20px;
}

.slide ul li {
  margin-bottom: 8px;
}

a {
  color: #7fb1ff;
  text-decoration: none;
  transition: color 0.3s ease;
}

a:hover {
  color: #a3c4f3;
  text-decoration: underline;
}

.controls {
  margin-top: 30px;
  text-align: center;
}

button {
  background-color: #3a5a99;
  border: none;
  color: white;
  padding: 12px 22px;
  margin: 0 12px;
  font-size: 18px;
  border-radius: 6px;
  cursor: pointer;
  box-shadow: 0 4px 10px rgba(0,0,0,0.3);
  transition: background-color 0.3s ease;
  user-select: none;
}

button:hover {
  background-color: #2a4470;
}

button:focus {
  outline: 2px solid #7fb1ff;
  outline-offset: 2px;
}
