```js
"use strict";

const { promises: { readFile } } = require("fs");
const xml2js = require('xml2js');


readFile('index.js', 'utf-8')
  .then(readed_file => {
    return readed_file
  })
  .then(xmlObj => {
    console.log(xmlObj);
  })
  .catch(my_error);


function my_error(error) {
  console.error(error.message);
  process.exit(1);

}

/*const fs = require('fs');

const test = fs.readFile('./source/MT_Yandex_en-ru_Learn-You-a-Haskell-for-Great-Good.tmx', 'utf-8', (err, data) => {
  if (err) {
    throw err;
  } else {
    console.log("Файл успешно прочитан\n");
    return '12312312';
  }
});
console.log(test);

function parse(xmlData) {
  let obj = {};
  xml2js.parseString(xmlData, (err, result) => {
    if (err) {
      console.error(err);
    } else {
      obj = result;
    }
  });
  return obj;
}

function main(xmlObj) {
  let xmlObj_mod = xmlObj;
  console.log(xmlObj)
  console.log(xmlObj.tmx.body[0].tu[0].tuv);
  let countT = 0;
  xmlObj.tmx.body[0].tu.forEach(item => {
    countT +=
      item.tuv[0].seg[0] == '' &&
        item.tuv[1].seg[0] == ''
        ? 1
        : 0
  });
  console.log(countT);
  return xmlObj_mod;
}

function write(path, data) {
  fs.writeFile('./dist/out.tmx', data, (err) => {
    if (err) {
      console.log(err);
    } else {
      console.log("Файл успешно записан\n");
    }
  });
}*/

```