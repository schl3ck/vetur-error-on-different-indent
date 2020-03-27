# vetur-error-on-different-indent
This is a sample repo to show the error 2551 of Vetur (VSCode extension)

## Steps
1. Clone the repo
2. Run `npm i`
3. Open the folder with VSCode and open the file `src/Errors.vue`
4. Wait until everything is loaded
5. Observe the error Veture(2551) on line 8 & 9 but not on line 10
6. Indent line 8 or 9 once => error still there
7. Indent same line again => error vanishes
8. Remove `(...)` from the function call on the other line => error vanishes
9. Add `()` to the function call on line 10 => error appears
