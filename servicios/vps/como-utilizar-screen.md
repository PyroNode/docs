# Cómo utilizar 'screen'

## ¿Qué es y para que sirve screen?

Screen es un administrador de ventanas en pantalla completa que permite tener varias terminales separadas en procesos distintos.

**En español:** Screen te permite tener varios programas abiertos en tu VPS sin tener que dejar tu conexión abierta.

## ¿Cómo se instala screen?

Instalar screen es muy sencillo, simplemente ejecuta el siguiente comando en tu VPS y listo, tendrás instalado screen en tu VPS.

```bash
sudo apt install screen
```

## ¿Cómo se utiliza screen?

Screen es un paquete muy completo y tiene demasiadas funciones en él pero nosotros te explicaremos las más básicas.

{% hint style="success" %}
Puedes investigar sus diversas funciones en su manual con `man screen`.
{% endhint %}

### Crear una nueva screen

Finalmente te has instalado screen pero no tienes ni idea de por donde empezar. ¿Cómo abres una screen?

Cuando quieras crear tu propia screen simplemente ejecuta `screen -S nombre`.

Una vez hecho eso, se te abrirá tu terminal "aislada" del resto. Podrás ejecutar cualquier programa/proceso dentro de ella que una vez te desconectes, seguirá activo.

{% hint style="info" %}
Para salir de una screen sin tener que desconectarte puedes utilizar **`Ctrl. + A`** y luego pulsar **`D`**.
{% endhint %}

### Volver a entrar en una screen

Has creado una screen, te desconectas de la VPS y ahora quieres volver a entrar a la screen que habías creado. ¿Cómo puedes hacerlo?

Para volver a entrar en una screen que habías creado, utiliza `screen -x nombre` y entrarás automáticamente.

### Ver listado de screens

Tienes 809 screens pero no te acuerdas de el nombre de la screen en la que tenías tu bot de fotos de gatitos. ¿Cómo encuentro el nombre?

Para ver listado de screens que tengas abiertas, ejecuta `screen -ls`. Te mostrará una lista de todas las screens que tengas abiertas en tu máquina.
