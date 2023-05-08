# IlkTurdaBitirelim
This app include gradle task. If you build this app, you can hear the sound.

## How to use gradle task?
### Add the following task to root/build.gradle

- w/KotlinDsl 

task("sayDone") {
    doLast {
        exec {
            commandLine("say", "Ilk Turda Bitirelim")
        }
    }
}

- w/Groovy

task sayDone {
    doLast {
        exec {
            commandLine 'say', 'Ilk Turda Bitirelim'
        }
    }
}

## Add gradle task to Before Launch in Edit Configuration



