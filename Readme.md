# Vladislav Pauliushchyk

![Me](https://github.com/plusch011/cv/blob/gh-pages/photo.jpg?raw=true)

**Position**: Front end developer  
**Experience**: 5 months  
**English**: A2+ - B1
**Education**: Molodchno State Musical College named M.K.Oginskogo(Opera singing)  
Belarusian State University of Informatics and Radioelectronics(Faculto of Information Technologies and Control 2.5 years)
**About me**: Able to work in team, responsible and attentive. I study music and art history. Love to sing, compose, play piano. Cheerful and sociable.  

## Professional skills

| Skill         | Experience    |
| ------------- |:-------------:|
| Javascript    | 6 months      |
| Git           | 6 month       |
| DOM           | 6 months      |
| React         | 2 month       |
| MobX          | 2 month       |

## Courses

**Epan RSS course (Front-end) ** Top 20.

## Projects

[Piskel clone(student project)](https://plusch011.github.io/piskel-clone/)  
[Youtube bootstrap(student project)](https://plusch011.github.io/youtube/)  

## Code examples

[Сodewars stats](https://www.codewars.com/users/plusch011/completed)

**Sudoku solver**  

```
function solveSudoku(sudoku, col = 0, row = 0, impsNum = []) {
	if (col > 8) col = 0, row++;
	if (row > 8) return sudoku;
	if (sudoku[row][col]) return solveSudoku(sudoku, col + 1, row) ? sudoku : false;
	for (let k = 0; k < 9; k++) {
		let kRow = Math.trunc(row / 3) * 3 + Math.trunc(k / 3);
		let kCol = Math.trunc(col / 3) * 3 + (k % 3);
		impsNum.push(sudoku[row][k], sudoku[k][col], sudoku[kRow][kCol]);
	}
	let posNum = [1, 2, 3, 4, 5, 6 ,7 ,8, 9].filter(elem => !impsNum.includes(elem));
	for (sudoku[row][col] of posNum) if (solveSudoku(sudoku, col + 1, row)) return sudoku;
	return sudoku[row][col] = 0;
}
```


