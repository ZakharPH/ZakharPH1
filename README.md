\documentclass[a4paper, 12pt]{article}

\usepackage[utf8]{inputenc}
\usepackage[T2A]{fontenc}
\usepackage[russian]{babel}

\usepackage[margin=2.2cm, top=1cm]{geometry}
\usepackage{amssymb,amsmath,amsthm,mathtools,hyperref}

\newtheorem{theorem}{Теорема}
\newtheorem{corollary}[theorem]{Следствие}
\newtheorem{lemma}[theorem]{Лемма}
\newtheorem{definition}[theorem]{Определение}

\theoremstyle{definition}
\newth
\newcommand{\N}{\mathbb{N}}       \newcommand{\Z}{\mathbb{Z}}  %\mathfrak{A}
\newcommand{\legendre}[2]{\ensuremath{\bigl( \frac{#1}{#2} \bigr)}} % \Bigl

\newcommand{\divsby}{%
   \mathrel{\:\rlap{.}\rlap{\raisebox{0.55ex}{.}}\raisebox{1.1ex}{.}\:}}eorem{problem}{Задача}


\begin{document}

\begin{flushright}
  {\it Матиматика,}\\
  {\it 21.12.2024}\\
  --- З. Т. Пидласко
\end{flushright}




\begin{problem}[{\bf Теорема Вильсона}] Доказать, что,
 \[(p - 1)! +1 \divsby p \Leftrightarrow\: (p \text{ --- простое число}).\]                  
\end{problem}



   {\bf Решение.} В задаче 2.5г доказана достаточность услловия <<p --- простое >>. Осталось доказать его необходимость.
Предположим противное: p --- состовное. Тогда среди чисел, меньших p, есть делители p. Если n и p/n --- два таких делителя, то они обавходят множителями в (p - 1)!, а значит, (p-1)! \(\divsby \perp\) p. Поэтому (p - 1)!+1\(\perp\) p.  

    Мы разобрали все случаи сократимости коэффицентов сравнения. Теперь самое время разобрать с несократимым случаем.

   Остаток a (mod b) назовём <<обратимым>>, если существует обратный к нему остаток, то есть такой \(a^{\prime}\), для которого \(aa^{\prime} \equiv 1\)(mod b). Для \(a^{\prime}\) мы будем использовать обозначение 1/а.

   \begin{problem} а) Докажите, что если a \(\perp\) b, то остаток a обратим.

   б) Докажите,что если остаток a (mod b) обратим, то a \(\perp\) b.

   в) Докажите, что если a \(\perp\) b, то решение сравнения ax \(\equiv\) c (mod b) является c/a (mod b), то есть c \(\cdot\) (1/a).

\end{problem}

   {\bf Решение.} а) Если a \(\perp\) b, то (по основной лемме из занятие 6 книги ДПЧ) существуют такие целые числа x и y, что ax + by = 1. Это значит, что ax \(\equiv\) 1 (mod b), то x = 1/a.

   б) Если \(aa^{\prime} \equiv\) 1 (mod b), то существует целое k, для которого \(aa^{\prime} \) - 1 = kb, \(aa^{\prime} \) - kb = 1.
 Любой общий делитель чисел a и b делит и выражение \(aa^{\prime} \), а значит, НОД(a,b) = 1, то есть a \(\perp\) b.

   в) Домножим обе части сравнения на 1/a. Получим равносильное сравнение(кстати,почему оно равносильно, а не является неравносильным следствием?):
\begin {center}
  (1/a)ax \(\equiv\) (1/a)c (mod b),
\end{center}
то есть x \(\equiv\) c/a \ (mod b).


\end{document}

