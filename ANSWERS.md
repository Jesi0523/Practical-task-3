# QUESTIONS AND ANSWERS

## ENGLISH

1. What does the `visible` prop of `Modal` do and why do we control it with `useState`?

- The `visible` prop makes it possible to show or hide the modal. It is controlled with `useState` because it is only shown if the user performs an action like clicking a button.

2. What is `onRequestClose` for? What happens on Android if you do not close the modal in it?

- The `onRequestClose` prop is used to close the `Modal` with the operating system's back button. On Android, without this function, the user will not be able to close the modal using that button.

3. What is the effect of `transparent={true}`? Name the three values of `animationType`.

- The `transparent={true}` prop allows us to remove the white background that the `Modal` has by default. The 3 values for `animationType` are `none`, `slide`, and `fade`.

4. Why does `ScrollView` exist? What happens with a long `View` without it? When would you choose `FlatList` instead?

- `ScrollView` allows us to see the other components that do not fit on the screen. If a `View` does not use it, the user will not be able to see the content that gets cut off due to the size of the phone screen. I would choose to use `FlatList` when I have to display too much data.

5. What is the difference between the `style` and the `contentContainerStyle` props of a `ScrollView`?

- The difference is that `style` is used to apply styles to the `ScrollView` itself, while `contentContainerStyle` is used to apply styles to the inner container that wraps the child elements.

6. What is `SafeAreaView` for and which zones of the device does it protect? Why do we use `react-native-safe-area-context`?

- `SafeAreaView` ensures that all the content we develop does not cover the edges of the phone, such as the time or the navigation buttons. We use `react-native-safe-area-context` because the native `SafeAreaView` from React Native only works on iOS, and with `react-native-safe-area-context` it also works on Android.

7. Write the three best practices from the Step 5 checklist in your own words and give an example of when a modal is **not** a good idea.

- Each screen should only have 1 modal and it must be concise.
- To display a lot of data it is better to use `FlatList`, since `ScrollView` is limited.
- Your screen should be wrapped inside a `SafeAreaView` to respect the edges of the phone.
- It is **not** a good idea to use a `Modal` when showing multiple alerts or when one modal appears after another and so on.

## ESPAÑOL

1. ¿Qué hace la propiedad `visible` de `Modal` y por qué la controlamos con `useState`?

- La propiedad `visible` hace que el modal se pueda ver u ocultar. Se controla con `useState` porque solamente se muestra si el usuario realizó alguna acción como darle click a un botón.

2. ¿Para qué sirve `onRequestClose`? ¿Qué sucede en Android si no cierras el modal dentro de esta función?

- La propiedad `onRequestClose` sirve para poder cerrar el Modal con el botón de regreso del sistema operativo. En Android sin esa función, el usuario no podrá cerrar el modal con ese botón.

3. ¿Cuál es el efecto de `transparent={true}`? Nombra los tres valores posibles para `animationType`.

- El efecto `transparent={true}` permite quitar el fondo blanco que tiene el `Modal`. Los 3 valores para `animationType` son `none`, `slide` y `fade`

4. ¿Por qué existe `ScrollView`? ¿Qué ocurre con un `View` largo si no se utiliza? ¿Cuándo elegirías usar `FlatList` en su lugar?

- El `ScrollView` nos permite ver los otros componentes que no caben en la pantalla. Si un `View` no lo usa, el usuario no podrá ver el contenido que se corta debido al tamaño de la pantalla del celular. Elegiría usar `FlatList` cuando tengo que mostrar demasiados datos. 

5. ¿Cuál es la diferencia entre la propiedad `style` y `contentContainerStyle` en un `ScrollView`?

- La diferencia es que `style` se usa para aplicar estilos al mismo ScrollView, mientras que `contentContainerStyle` se usa para aplicar estilos al contenedor interno que envuelve a los elementos hijos.

6. ¿Para qué sirve `SafeAreaView` y qué zonas del dispositivo protege? ¿Por qué utilizamos `react-native-safe-area-context`?

- `SafeAreaView` sirve para que todo el contenido que desarrollemos no tape los bordes que hay en el celular, como la hora o los botones de navegación. Usamos `react-native-safe-area-context` porque el `SafeAreaView` nativo de React Native solo funciona en iOS y con `react-native-safe-area-context` también funciona para Android.

7. Escribe con tus propias palabras las tres buenas prácticas de la lista de verificación del Paso 5 y da un ejemplo de cuándo un modal **no** es una buena idea.

- En cada pantalla debe de haber solamente 1 modal y debe ser conciso.
- Para mostrar muchos datos es mejor usar `FlatList`, ya que `ScrollView` está limitado.
- Tu pantalla debe de estar dentro de un `SafeAreaView` para respetar los bordes del celular.
- **No** es buena idea usar un `Modal` cuando muestras varios avisos o también cuando aparece un modal y luego otro y asi sucesivamente.