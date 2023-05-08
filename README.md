# IlkTurdaBitirelim
![Kotlin](https://img.shields.io/badge/kotlin-%230095D5.svg?style=for-the-badge&logo=kotlin&logoColor=white)
![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)
![Android Studio](https://img.shields.io/badge/Android%20Studio-3DDC84.svg?style=for-the-badge&logo=android-studio&logoColor=white)
![Gradle](https://img.shields.io/badge/Gradle-02303A.svg?style=for-the-badge&logo=Gradle&logoColor=white)

This app include gradle task. If you build this app, you can hear the sound.

## Gradle Task Sound
https://user-images.githubusercontent.com/37421570/236877541-46513876-fc11-4e87-b81d-b75328014446.mp4


## How to use gradle task?
Add the following task to root/build.gradle 👇🏻

- `w/KotlinDsl`

```
task("sayDone") {
    doLast {
        exec {
            commandLine("say", "Ilk Turda Bitirelim")
        }
    }
}
```

- `w/Groovy`

```
task sayDone {
    doLast {
        exec {
            commandLine 'say', 'Ilk Turda Bitirelim'
        }
    }
}
```

## Add gradle task to Before Launch in Edit Configuration
<p>
 <img align="center" src="gradle_task.png" height="550"/>
</p>


