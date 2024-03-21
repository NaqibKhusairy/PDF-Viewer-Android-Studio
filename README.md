PDF Viewer Android Studio
This project is an Android application that allows users to view PDF files within the app. It utilizes the com.github.barteksc:android-pdf-viewer library.

Setup
1. Add the following dependency to the build.gradle file (Module: app):

*For beta version:
implementation 'com.github.barteksc:android-pdf-viewer:3.2.0-beta.1'

*For stable version:
implementation 'com.github.barteksc:android-pdf-viewer:2.8.2'

2. Add the following dependency to the build.gradle file (Project: {Project Name}):
buildscript {
    dependencies {
        classpath 'com.google.gms:google-services:4.3.14'
        classpath 'com.android.tools.build:gradle:7.2.0'
    }
}

3. Enable Jetifier in the gradle.properties file:
android.enableJetifier=true

4. Add jcenter() to the settings.gradle file.

Usage
Include PDFView in your layout XML file:

<com.github.barteksc.pdfviewer.PDFView
    android:id="@+id/pdfView"
    android:layout_width="match_parent"
    android:layout_height="match_parent"/>

You can now use PDFView in your activity to display PDF files.
