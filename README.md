/* Global styles */
* {
  box-sizing: border-box;
}

body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0 10px;
}

h1 {
  text-align: center;
  font-size: 2em;
  margin-top: 20px;
  margin-bottom: 40px;
}

/* Section styles */
.section {
  border: 1px solid black;
  background-color: #f9f9f9;
  padding: 40px 10px 10px 10px;
  margin: 10px;
  position: relative;
  float: left;
  width: 100%;
}

.section-title {
  position: absolute;
  top: 0;
  right: 0;
  background-color: #e0e0e0;
  border: 1px solid black;
  padding: 5px 10px;
  font-size: 1.25em;
}

/* Custom colors for each title */
.chicken {
  background-color: #ffcccb;
}

.beef {
  background-color: #d5a6bd;
}

.sushi {
  background-color: #c4d79b;
}

/* Desktop view (≥ 992px) */
@media (min-width: 992px) {
  .section {
    width: 31.33%;
    margin: 1%;
  }
}

/* Tablet view (768px–991px) */
@media (min-width: 768px) and (max-width: 991px) {
  .section {
    float: none;
    margin: 10px auto;
  }

  .section:nth-child(1),
  .section:nth-child(2) {
    width: 47%;
    float: left;
    margin: 1%;
  }

  .section:nth-child(3) {
    width: 96%;
    clear: both;
  }
}

/* Mobile view (≤ 767px) */
@media (max-width: 767px) {
  .section {
    width: 100%;
    float: none;
    margin-bottom: 20px;
  }
}
