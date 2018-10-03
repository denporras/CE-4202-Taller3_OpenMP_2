# CE-4202-Taller3_OpenMP_2
En este taller se estudiará implementación de paralelismo a partir de un código secuencial en C, utilizando la extensión de OpenMP para dispositivos móviles multiprocesador basados en Android.

# Intrucciones

Antes de ejecutar los programas se debe conectar el telefono Android en modo de depuración USB.

## SAXPY serial

1- Abrir la terminal en la carpeta:
	saxpy/

2- Compilar con el siguiente comando: 
  ```console
  usuario@Computer:~$ /opt/android-ndk-r16b/ndk-build

  ```
3- Entrar en la carpeta **jni**:
  ```console
  usuario@Computer:~$ cd jni/

  ```
4- Agregar el ejecutable al telefono:
  ```console
  usuario@Computer:~$ adb push ../libs/armeabi-v7a/saxpy /data/local/tmp

  ```
5- Ejecutar el programa:
  ```console
  usuario@Computer:~$ adb shell /data/local/tmp/saxpy

  ```

## SAXPY paralelo

1- Abrir la terminal en la carpeta:
	saxpy_par/

2- Compilar con el siguiente comando: 
  ```console
  usuario@Computer:~$ /opt/android-ndk-r16b/ndk-build

  ```
3- Entrar en la carpeta **jni**:
  ```console
  usuario@Computer:~$ cd jni/

  ```
4- Agregar el ejecutable al telefono:
  ```console
  usuario@Computer:~$ adb push ../libs/armeabi-v7a/saxpy_par /data/local/tmp

  ```
5- Ejecutar el programa:
  ```console
  usuario@Computer:~$ adb shell /data/local/tmp/saxpy_par
  
  ```