<template lang="pug">
  .curso-main-container.pb-3
    BannerInterno(icono="far fa-question-circle" titulo="Actividad didáctica")
    .container.tarjeta.tarjeta--blanca.p-4.p-md-5
      // Para cuestionario usar: ActividadController(:cuestionario="cuestionario") 
      // Para parrafo usar: ActividadController(:parrafo="parrafo")
      ActividadController(:cuestionario="cuestionario")
  </template>

<script>
import ActividadController from '@ecored-sena/base-kit/plugin/components/actividad/ActividadController.vue'

export default {
  name: 'ActividadDidactica',
  components: {
    ActividadController,
  },
  data: () => ({
    cuestionario: {
      tema: 'Nombre del CF',
      titulo: 'Cuestionario',
      introduccion:
        '<b> Objetivo:</b> verificar la comprensión de los conceptos fundamentales relacionados con la preparación del entorno de desarrollo, la arquitectura de servidores Node.js y la implementación de comunicación en tiempo real mediante WebSockets',
      barajarPreguntas: true,
      titulo_aprobado: '¡BUEN TRABAJO!',
      titulo_reprobado: 'VUELVA A INTENTARLO.',
      preguntas: [
        {
          id: 1,
          texto:
            '¿Cuál\tes\tel propósito principal de Node.js en el desarrollo web?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Ejecutar JavaScript en el servidor.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Diseñar interfaces gráficas.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los conceptos fundamentales abordados en el componente formativo.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente el componente formativo e intentar nuevamente la actividad.',
        },
        {
          id: 2,
          texto:
            '¿Qué archivo se genera al inicializar un proyecto con npm init?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'index.html.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'package.json.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los conceptos fundamentales abordados en el componente formativo.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente el componente formativo e intentar nuevamente la actividad.',
        },
        {
          id: 3,
          texto: '¿Cuál es la función principal del framework Express.js?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Crear bases de datos.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Administrar el sistema operativo.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los conceptos fundamentales abordados en el componente formativo.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente el componente formativo e intentar nuevamente la actividad.',
        },
        {
          id: 4,
          texto: '¿Qué permite el protocolo WebSocket en aplicaciones web?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Transferir archivos únicamente.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Enviar datos solo mediante HTTP.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los conceptos fundamentales abordados en el componente formativo.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente el componente formativo e intentar nuevamente la actividad.',
        },
        {
          id: 5,
          texto:
            '¿Qué técnica se utilizaba tradicionalmente antes de WebSockets para consultar información del servidor?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Long polling.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Broadcast.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los conceptos fundamentales abordados en el componente formativo.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente el componente formativo e intentar nuevamente la actividad.',
        },
        {
          id: 6,
          texto:
            '¿Qué biblioteca se utiliza comúnmente para implementar WebSockets en Node.js?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Angular.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Socket.io.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los conceptos fundamentales abordados en el componente formativo.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente el componente formativo e intentar nuevamente la actividad.',
        },
        {
          id: 7,
          texto: '¿Qué función cumple el event loop en Node.js?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Crear interfaces de usuario.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Almacenar datos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los conceptos fundamentales abordados en el componente formativo.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente el componente formativo e intentar nuevamente la actividad.',
        },
        {
          id: 8,
          texto:
            '¿Qué comando se utiliza para instalar dependencias en Node.js?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'node install.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'node run.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los conceptos fundamentales abordados en el componente formativo.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente el componente formativo e intentar nuevamente la actividad.',
        },
        {
          id: 9,
          texto: '¿Qué representa el objeto socket en Socket.io?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Una conexión específica entre cliente y servidor.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Un archivo de configuración.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los conceptos fundamentales abordados en el componente formativo.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente el componente formativo e intentar nuevamente la actividad.',
        },
        {
          id: 10,
          texto:
            '¿Qué método permite enviar un mensaje a todos los clientes conectados?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'socket.listen().',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'server.send().',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los conceptos fundamentales abordados en el componente formativo.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente el componente formativo e intentar nuevamente la actividad.',
        },
        {
          id: 11,
          texto: '¿Qué función cumple un IDE en el desarrollo de software?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Facilitar la escritura, depuración y ejecución del código.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Reemplazar el sistema operativo.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los conceptos fundamentales abordados en el componente formativo.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente el componente formativo e intentar nuevamente la actividad.',
        },
        {
          id: 12,
          texto:
            '¿Qué ventaja ofrece Visual Studio Code en el desarrollo con Node.js?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Eliminación del código JavaScript.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Sustitución del servidor.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los conceptos fundamentales abordados en el componente formativo.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente el componente formativo e intentar nuevamente la actividad.',
        },
        {
          id: 13,
          texto: '¿Qué significa que HTTP sea un protocolo stateless?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Que mantiene todas las conexiones activas.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Que solo funciona en tiempo real.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los conceptos fundamentales abordados en el componente formativo.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente el componente formativo e intentar nuevamente la actividad.',
        },
        {
          id: 14,
          texto:
            '¿Qué tipo de comunicación permite enviar y recibir datos simultáneamente?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Half-duplex.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Single-thread.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los conceptos fundamentales abordados en el componente formativo.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente el componente formativo e intentar nuevamente la actividad.',
        },
        {
          id: 15,
          texto: '¿Qué representa el puerto 3000 en un servidor Node.js?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto:
                'Un punto de conexión de red donde el servidor escucha peticiones.',
              esCorrecta: true,
            },
            {
              id: 'b',
              texto: 'Una base de datos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los conceptos fundamentales abordados en el componente formativo.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente el componente formativo e intentar nuevamente la actividad.',
        },
        {
          id: 16,
          texto: '¿Qué función cumple el método require() en Node.js?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Ejecutar código HTML.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Importar módulos al programa.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los conceptos fundamentales abordados en el componente formativo.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente el componente formativo e intentar nuevamente la actividad.',
        },
        {
          id: 17,
          texto: '¿Qué ventaja ofrece la arquitectura asincrónica de Node.js?',
          imagen: require('@/assets/actividad/imagen1.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Reduce la velocidad del servidor.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Limita el uso de eventos.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los conceptos fundamentales abordados en el componente formativo.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente el componente formativo e intentar nuevamente la actividad.',
        },
        {
          id: 18,
          texto:
            '¿Qué tipo de aplicaciones se benefician más del uso de WebSockets?',
          imagen: require('@/assets/actividad/imagen2.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Aplicaciones estáticas.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Archivos PDF.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los conceptos fundamentales abordados en el componente formativo.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente el componente formativo e intentar nuevamente la actividad.',
        },
        {
          id: 19,
          texto:
            '¿Qué herramienta permite gestionar dependencias en proyectos Node.js?',
          imagen: require('@/assets/actividad/imagen3.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'MySQL.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'npm.',
              esCorrecta: true,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los conceptos fundamentales abordados en el componente formativo.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente el componente formativo e intentar nuevamente la actividad.',
        },
        {
          id: 20,
          texto:
            '¿Qué competencia desarrolla el aprendiz al construir aplicaciones en tiempo real?',
          imagen: require('@/assets/actividad/imagen4.png'),
          barajarRespuestas: true,
          opciones: [
            {
              id: 'a',
              texto: 'Memorización de comandos.',
              esCorrecta: false,
            },
            {
              id: 'b',
              texto: 'Reducción de código.',
              esCorrecta: false,
            },
          ],
          mensaje_correcto:
            'Se evidencia comprensión de los conceptos fundamentales abordados en el componente formativo.',
          mensaje_incorrecto:
            'Se recomienda revisar nuevamente el componente formativo e intentar nuevamente la actividad.',
        },
      ],
      mensaje_final_aprobado: '¡Excelente! Ha superado la actividad.',
      mensaje_final_reprobado:
        'Le recomendamos volver a revisar el componente formativo e intentar nuevamente la actividad didáctica.',
    },
  }),
}
</script>
