# Notes-Learning-Android-

Challenges of developing Apps
\*Availability

- Performance (Unfortunately, kobo has stopped)
  ----> Quality

1. Know the Operating System
2. The versions of the Operating system (Choose based on% of use)
3. Android Screen Densities
4. Performance (Memory usage and CPU consumption)
5. Design Metrics (Material Design)
6. Development environment
7. Testing

Types of Android devices and Support
     Each android device hardware has an ID to be invoked
     example: FEATURE_CAMERA_FRONT, FEATURE_NFC, FEATURE_SENSOR_STEP_COUNTER, FEATURE_MICROPHONE

    minSdkVersion 15 to be classified in play store
    targetSdkVersion 26 is the target version with which the app is 100% compatible but still compatible with the 28.29

#Activity (Class Java hereda de la clase Activity + XML layaut)
#Cicle life to Activity
![alt text](cicleLifeActiviy.png)

- In method create save state of Activity
- onResumen() The activity has become visible
- onPause() "partially Visible" Another activity is taking focus(this activity is about to be "paused")
- onStop() The activity is no longer visible, this happens when you press home
- onDestroy() the activity is destroy

In Spanish
onCreate(Bundle): Se llama en la creación de la actividad. Se utiliza para realizar todo tipo de inicializaciones, como la creación de la interfaz de usuario o la inicialización de estructuras de datos. Puede recibir información de estado de la actividad (en una instancia de la clase Bundle), por si se reanuda desde una actividad que ha sido destruida y vuelta a crear.

onStart(): Nos indica que la actividad está a punto de ser mostrada al usuario.

onResume(): Se llama cuando la actividad va a comenzar a interactuar con el usuario.

onPause(): Indica que la actividad está a punto de ser lanzada a segundo plano, normalmente porque otra actividad es lanzada.

onStop(): La actividad ya no va a ser visible para el usuario.

onRestart(): Indica que la actividad va a volver a ser representada después de haber pasado por onStop().

onDestroy(): Se llama antes de que la actividad sea totalmente destruida. Por ejemplo, cuando el usuario pulsa el botón de volver o cuando se llama al método finish().

#Fragment
Used
-FragmentManager
-Transaction
-Commits

#Intent
In Spanish
Los Intents nos servirán para unir componentes de una aplicación, y podemos tener dos casos específiamente:

1. El que ya mencionamos, unir Activity’s dentro de la aplicación
2. Unir Activity’s que viven en diferentes aplicaciones

Los primeros se llamarán Explicitos
![alt text](1caseIntent.jpg)

Los segundos Implícitos
![alt text](2CaseIntent.jpg)
