# Prolog

## Calculadora de Áreas Geométricas en Lisp
Esta practica contiene un conjunto de funciones en Lisp que permiten calcular el área de diversas formas geométricas, como cuadrados, triángulos, círculos, pentágonos, hexágonos, trapecios, rombos, cubos y esferas. Estas funciones son útiles para realizar cálculos de áreas de formas comunes en matemáticas y geometría.

Cada función en este programa solicita información específica al usuario, como medidas de lados, bases, alturas o radios, y luego utiliza fórmulas matemáticas para calcular el área correspondiente. Los resultados se muestran en la consola para que el usuario pueda ver el área calculada.
- **Función Cuadrado:** Esta función calcula el área de un cuadrado.
```lisp
(defun cuadrado()
    (princ "Area de un cuadrado: ")
    (terpri)
    (princ "Ingresa la medida de un lado: ")
    (setq lado(read))
    (setq resultado (* lado lado))
    (format t "Area del cuadrado: ~,2f~%" resultado)
    (terpri)
)
```

- **Función Triángulo:** Esta función calcula el área de un triángulo.
```lisp
(defun triangulo()
    (princ "Area de un triangulo: ")
    (terpri)
    (princ "Ingresa la medida de la base: ")
    (setq base(read))
    (princ "Ingresa la medida de la altura: ")
    (setq altura(read))
    (setq resultado (/ (* base altura) 2))
    (format t "Area del triangulo: ~,2f~%" resultado)
    (terpri)
)
```

- **Función Rectángulo:** Esta función calcula el área de un rectángulo.
```lisp
(defun rectangulo()
    (princ "Area de un rectangulo: ")
    (terpri)
    (princ "Ingresa la medida de la base: ")
    (setq base(read))
    (princ "Ingresa la medida de la altura: ")
    (setq altura(read))
    (setq resultado (* base altura))
    (format t "Area del rectangulo: ~,2f~%" resultado)
    (terpri)
)
```

- **Función Círculo:** Esta función calcula el área de un círculo.
```lisp
(defun circulo()
    (princ "Area de un circulo: ")
    (terpri)
    (princ "Ingresa la medida del radio: ")
    (setq radio(read))
    (setq resultado (* PI (* radio radio)))
    (format t "Area del circulo: ~,2f~%" resultado)
    (terpri)
)
```

- **Función Pentágono:** Esta función calcula el área de un pentágono regular.
```lisp
(defun pentagono()
    (princ "Area de un pentagono: ")
    (terpri)
    (princ "Ingresa la medida de un lado: ")
    (setq lado(read))
    (princ "Ingresa la apotema: ")
    (setq apotema (read))
    (setq resultado (* (/ 5 4) (* lado apotema)))
    (format t "Area del pentagono: ~,2f~%" resultado)
    (terpri)
)
```

- **Función Hexágono:** Esta función calcula el área de un hexágono regular.
```lisp
(defun hexagono()
    (princ "Area de un hexagono: ")
    (terpri)
    (princ "Ingresa la medida de un lado: ")
    (setq lado (read))
    (princ "Ingresa la apotema: ")
    (setq apotema (read))
    (setq resultado (* 3 (* lado apotema)))
    (format t "Area del hexagono: ~,2f~%" resultado)
    (terpri)
)
```

- **Función Trapecio:** Esta función calcula el área de un trapecio.
```lisp
(defun trapecio()
    (princ "Area de un trapecio: ")
    (terpri)
    (princ "Ingresa la medida de la base mayor: ")
    (setq base-mayor (read))
    (princ "Ingresa la medida de la base menor: ")
    (setq base-menor (read))
    (princ "Ingresa la medida de la altura: ")
    (setq altura (read))
    (setq resultado (* (/ (+ base-mayor base-menor) 2) altura))
    (format t "Area del trapecio: ~,2f~%" resultado)
    (terpri)
)
```

- **Función Rombo:** Esta función calcula el área de un rombo.
```lisp
(defun rombo()
    (princ "Area de un rombo: ")
    (terpri)
    (princ "Ingresa la medida de la diagonal mayor: ")
    (setq diagonal-mayor (read))
    (princ "Ingresa la medida de la diagonal menor: ")
    (setq diagonal-menor (read))
    (setq resultado (* (/ (* diagonal-mayor diagonal-menor) 2)))
    (format t "Area del rombo: ~,2f~%" resultado)
    (terpri)
)
```

- **Función Cubo:** Esta función calcula el área de un cubo.
```lisp
(defun cubo()
    (princ "Area de un cubo: ")
    (terpri)
    (princ "Ingresa la medida de un lado: ")
    (setq lado (read))
    (setq resultado (* 6 (* lado lado)))
    (format t "Area del cubo: ~,2f~%" resultado)
    (terpri)
)
```

- **Función Esfera:** Esta función calcula el área de una esfera.

```lisp
(defun esfera()
    (princ "Area de una esfera: ")
    (terpri)
    (princ "Ingresa el radio de la esfera: ")
    (setq radio (read))
    (setq resultado (* 4 pi (* radio radio)))
    (format t "Area de la esfera: ~,2f~%" resultado)
    (terpri)
)
```
