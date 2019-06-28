# Vladislav Pauliushchyk

![Me](https://github.com/plusch011/cv/blob/gh-pages/photo.jpg?raw=true)

**Position**: Front end developer  
**Experience**: 5 months  
**English**: A2+  
**Education**: Molodechno State Musical College named M.K.Oginskogo  
**About me**: Able to work in team, responsible and attentive.  

## Professional skills

| Skill         | Experience    |
| ------------- |:-------------:|
| Javascript    | 5 months      |
| DOM           | 4 months      |
| React         | 1 month       |
| MobX          | 1 month       |

## Projects

[Piskel clone(training project)](https://plusch011.github.io/TrainPiskel/)

## Code examples

[Сodewars stats](https://www.codewars.com/users/plusch011/completed)

* Sudoku solver *  

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

##### P.S. Im on RSS JS course now. My position after 2-nd stage is 10.
