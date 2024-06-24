# General standards for programming

1. Don't use non-standard commands (such as `\fp` for `\mathfrak{p}`).
1. On the `template.sty` at the very beginning there are some customizable
   commands, like `\algcl` for the algebraic closure.
1. Use `\dpage` for marking page breaks in the original document.
1. Updated notation should be given its own command for easy customization, it
   should go in _Editors' notes_ and it should be at the beginning of the
   `template.sty` file with the rest.
1. Preserve the maximum of 80 characters per line inside the main matter (in
   `template.sty` it may be exceeded).
1. For inline math use `$...$`, for display math use `\[...\]`.
1. Avoid the use of `\displaystyle` unless strictly necessary. If an equation
   is inline and too big, just make it display.
1. Use `\strong{...}` for definitions, and `\emph{...}` for highlights.
   **Never** use `\textbf` nor `\textit`.
1. Follow definitions with `\index{}`.
1. Use the environments `thm` for theorem, `lem` for lemma, `prop` for
   proposition, `mydef` for definition, `obs` for remarks and `ex` for
   examples.  
   Corollaries are complicated: use `cor` after `thm`, `corl` after `lem`
   and `corp` after `prop` (the numbering is dependent on those).
1. Always use `\ref{...}` (or similars) for in-document citations.  
   Theorem 3 of subsection 2.4 of chapter I is labeled as `\label{thm:I_24_3}`.
1. Abreviations followed by letters should be separated with the `\ `
   command. For example _cf. Weil_ should be `cf.\ Weil`.
1. Numbered statements should be separated by `~`. For example, _See prop. 2_
   should be `See prop.~2`.
1. Exercise(s) don't have their dedicated environment, instead they are
   considered starred subsubsections.
1. Serre's entry _[24], p. 13_ is cited as `\cite[13]{24}`.
1. For tasks we use the `todonotes` package! (Check the `template.sty` for
   common styles.)
