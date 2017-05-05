<h6> kotlin-for-android-studio</h6>
1.install plugin for Android Studio.File>Settings>(Plugins>Browse Repositories>search Kotlin>Install)|(Install plugin from disk...>download from:<a href="https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-compiler-embeddable/">https://jcenter.bintray.com/org/jetbrains/kotlin/kotlin-compiler-embeddable/... .zip</a>)>restart IDE
2.Creating a project from Android Studio and Converting Java code to Kotlin like sample:<a href="http://kotlinlang.org/docs/tutorials/kotlin-android.html">http://kotlinlang.org/docs/tutorials/kotlin-android.html</a>
3.Choose Help | Find Action on the main menu or press Ctrl+Shift+A. 
4.Converti Java code to Kotlin press Ctrl+Alt+Shift+K
5.Configuring Kotlin in the project.edit .kt file,show>Kotlin is not configured>Configure>Android with Gradle>All modules containing Kotlin files>choose version from Kotlin compiler and runtime version>OK
6.Sync Now.Projec build.gradle>buildscript>dependencies>classpath "org.jetbrains.kotlin:kotlin-gradle-plugin:$kotlin_version" And Modules build.gradle>apply plugin: 'kotlin-android'>dependencies>compile "org.jetbrains.kotlin:kotlin-stdlib-jre7:$kotlin_version"
7.Kotlin Android Extensions.Configuring the dependency>add modules build.gradle apply plugin: 'kotlin-android-extensions'>import kotlinx.android.synthetic.main.<layout.name>.*>this.id.method
