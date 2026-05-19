# 

# 

# 

# 

# 

# **Auditoría ASG**

**Módulo:Sostenibilidad**   
   **Profesor:Willman Acosta Lugo**  
   **Autores: Juan Luis Nuñez y Lucas Moreno**   
**Empresa: Mercadona**

## Fase 1: Inventario y Dimensión Ambiental (A)

Analiza el peso y consumo de la web elegida.

1. **Medición inicial**. Utiliza herramientas gratuitas como *Website Carbon Calculator* o *Lighthouse* (pestaña de rendimiento en Chrome/Edge) para obtener la huella de carbono estimada por visita.  
   <img width="582" height="479" alt="image" src="https://github.com/user-attachments/assets/445e7610-c18b-4f39-bd7b-9e53ec713dd2" />
   
   Está bastante bien pero es mejorable.  
2. **Identificación de Bloatware**. Inspecciona la red (Network) en las herramientas de desarrollador del navegador. Identifica los 3 recursos más pesados que se descargan al abrir la web (imágenes sin comprimir, vídeos de fondo, librerías JavaScript pesadas, etc.).  
   Estas son los 3 recursos más pesados de la web   
   <img width="484" height="63" alt="image" src="https://github.com/user-attachments/assets/1b63cb72-5699-48b0-8818-df8aa99347d7" />
  
     
3. **Análisis**. ¿Crees que la web sufre de "inflación de software"? Justifica tu respuesta.

   Sí, un poco, Mercadona tiene mucha complejidad tecnológica interna, pero parece bastante enfocada en evitar exceso de herramientas y costes innecesarios. Esto se ve simplemente fijándonos en que es simple a propósito,priorizan eficiencia antes que hacer cosas para que se vea moderna tanto la web como la app.

## Fase 2: Dimensión Social y Equidad (S)

La web debe ser utilizable por todos. Evalúa la accesibilidad (Sostenibilidad Social):

1. **Test de Accesibilidad**. Pasa una herramienta como *WAVE Web Accessibility Evaluation Tool* o el propio *Lighthouse* (pestaña *Accessibility*).

	<img width="569" height="394" alt="image" src="https://github.com/user-attachments/assets/0be89608-e0b4-4cd9-b9b0-e1eb4df98bd8" />


<img width="545" height="449" alt="image" src="https://github.com/user-attachments/assets/a1db64c0-fa27-4ef5-a50e-27d6465111ad" />


El rendimiento es mejorable aunque comparado con accesibilidad, práctica y SEO la web no está tan mal 

2. **Identificación de barreras**. Documenta al menos 2 problemas graves que impidan a personas con diversidad funcional usar la web correctamente (ej. falta de atributos *alt* en imágenes clave, bajo contraste de colores en botones, formularios sin etiquetas).  
   Que las imágenes de producto no tienen un texto en el que se explique para que así el cliente le quede todo más claro.  
   Si tardas mucho en elegir los productos la sesión se cierra sola por seguridad sin avisar claramente.

	

## 

## 

## Fase 3: Dimensión de Gobernanza y Ética (G)

Revisa cómo trata la empresa a sus usuarios y sus datos:

1. **Transparencia**. ¿Es fácil rechazar las cookies no esenciales o utilizan "patrones oscuros" (Dark Patterns) para forzar al usuario a aceptarlas?  
   Sí. Al entrar en su web informativa (info.mercadona.es), el aviso de cookies nos da a elegir entre tres opciones claras y  visibles con el mismo nivel de jerarquía visual:"Rechazar", "Configurar" y "Aceptar".  
2. **Datos innecesarios**. ¿Pide la web datos personales excesivos en su formulario de contacto o registro?  
   No pide datos de más: no solicita información irrelevante (como género, estado civil, profesión o DNI).  
   Formulario de contacto: Solo pide lo básico para responder (Nombre, Email, Teléfono).  
   Registro de compra: Solo solicita los datos estrictamente necesarios para el reparto y la factura (Nombre, Dirección, Teléfono, Email y Código Postal).

## Fase 4: Propuesta de Refactorización (Green Coding)

Como desarrollador/a, no basta con encontrar los fallos; debes proponer soluciones. Redacta una propuesta de mejora técnica detallando:

* **Optimización de activos**.   
  * ¿Qué formatos usarías para sustituir las imágenes actuales (ej. WebP, AVIF)?   
    Hay que pasar de fotos viejas a AVIF o WebP porque pesan poquísimo y se ven muy bien así que la página cargaría muy rápido.  
  * ¿Implementarías Lazy Loading?  
    Si porque para que cargar algo que a lo mejor no vas ni a ver, asi solo descarga la imagen cuando haces scroll en ellas.  
* **Reducción de peticiones**.  
  * ¿Qué librerías o scripts externos eliminarías o aplazarías para mejorar la eficiencia del código y reducir el procesamiento en el dispositivo del cliente?  
    Si ponemos un modo oscuro (Dark Mode) opcional, el móvil del cliente consume mucha menos batería al navegar ahi.

* **Reflexión sobre la Paradoja de Jevons**.  
  * Si optimizamos la web y la carga mucho más rápido, podríamos atraer a muchos más usuarios diarios. ¿Cómo evitarías que este éxito anule el ahorro energético conseguido?  
    Haría:   
    Usaría servidores que sean 100 % renovables en el que se apaguen cuando no esté en uso.  
    También borrar datos antiguos que no sirvan para nada.  
      
