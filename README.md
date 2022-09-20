
<p align="center">
<img src="/testfood.png" width="15%"/>
<h1 align="center">thegoodchef - Food Recipes App</h1>
</p>

<p align="center">
  <a href="https://opensource.org/licenses/Apache-2.0"><img alt="License" src="https://img.shields.io/badge/License-Apache%202.0-blue.svg"/></a>
  <a href="https://android-arsenal.com/api?level=24"><img alt="API" src="https://img.shields.io/badge/API-21%2B-brightgreen.svg?style=flat"/></a>
  <a href="https://github.com/michaelmartinezw"><img alt="Profile" src="https://img.shields.io/static/v1?label=GitHub&message=michael&color=E53935"/></a>
</p>

<p align="center">  
thegoodchef es una app de prueba de android moderno.
</br>

## Descarga

Ir a  [Releases](https://github.com/michaelmartinezw/thegoodchef/releases) para poder descargar el apk.

<img src="previews/preview.gif" align="right" width="20%"/>

## Librerias

SDK mínimo nivel 2

- [Kotlin](https://kotlinlang.org/) based, [Coroutines](https://github.com/Kotlin/kotlinx.coroutines) + [Flow](https://kotlin.github.io/kotlinx.coroutines/kotlinx-coroutines-core/kotlinx.coroutines.flow/)

- Hilt (alpha) para inyección de dependencia.

- JetPack

- LiveData: notifique los datos de la capa de dominio a las vistas.
- Ciclo de vida: deseche los datos de observación cuando cambie el estado del ciclo de vida.

- ViewModel: titular de datos relacionados con la interfaz de usuario, consciente del ciclo de vida.
Persistencia de la sala: construya una base de datos utilizando la capa abstracta.

- Arquitectura MVVM ( View - DataBinding - ViewModel - Model)

- Patrón de repositorio

- [Retrofit2 & OkHttp3](https://github.com/square/retrofit) : constructor de API REST y  paginación  de datos de la red.

- [Gson](https://github.com/square/gson/): una biblioteca JSON moderna para Kotlin y Java.

- [Glide](https://github.com/bumptech/glide) - control de imágenes.

- [Material-Components](https://github.com/material-components/material-components-android): componentes de diseño de materiales como animación ondulada, cardView.

Vistas personalizadas

- [ShimmerRecyclerView](https://github.com/omtodkar/ShimmerRecyclerView): un Shimmer RecyclerView personalizado que adopta la transición de lista/cuadrícula automáticamente y también admite múltiples tipos de vista mientras brilla.

- [RoundedImageView](https://github.com/vinc3m1/RoundedImageView): un ImageView rápido que admite esquinas redondeadas, óvalos y círculos.

- [RealtimeBlurView](https://github.com/mmin18/RealtimeBlurView): una superposición de desenfoque en tiempo real para Android (como iOS UIVisualEffectView).

- [LottieFiles](https://lottiefiles.com/blog/working-with-lottie/getting-started-with-lottie-animations-in-android-app): muestre animaciones de Lottie livianas, escalables e interactivas en sus sitios web y aplicacion

## Arquitectura

Appita is based on MVVM architecture and a repository pattern.

![architecture](https://developer.android.com/topic/libraries/architecture/images/final-architecture.png)

## Open API

<img src="https://spoonacular.com/images/spoonacular-logo-b.svg" align="right" width="10%"/>

thegoodchef (Recipes App) utiliza [Spoonacular API](https://spoonacular.com/food-api) para realizar una RESTful API.<br>
Spoonacular API provee una RESTful API interface de objetos muy detallados creados a partir de miles de líneas de datos relacionados con recetas.
## Previo al Desarrollo
-Para la utilización de la API [Spoonacular API](https://spoonacular.com/food-api) se creo un perfil para obtener la APIKEY 
-Lectura detallada de la documentación para el armado de la arquitectura y de las rutas a implentar para realizar  queries y peticiones a los endpoint.
## En Desarrollo
-1 Creaercion del proyecto con kotlin como lengiaje 
-2 Implementación de librerias
-3 Armado de la arquitectura MVVM
-4 Confección de UI #corutinas #databinding
-5 Confección de modelos BD con ROOM 
-6 Confección de interface con retoffit para realizar las peticiones a los endpoint 
-7 Inyección de depndecia en las clases requeridas #dagger
-8 Testing y debugs errores 
-9 Confección de documento y Upload a GITHUB

# Problemas durante el desarrollo

Problemas con la implementacion de databinding  kapt "androidx.databinding:databinding-common:4.1.2"

Solucion: 
Se habilito android.enableJetifier=true en gradel.propierties

```xml
Compilado por Michael W. Martinez
