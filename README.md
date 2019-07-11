# Ud2_Ejemplo6
_Ejemplo 6 de la Unidad 2._

Vemos un ejemplo de cómo trabajar con pesos en el ViewGroup _LinearLayout_ usando el atributo _layout_weight_. Modificando su valor podemos ver cómo el tamaño asignado a ese _TextView_ cambia.

Sólo hemos de fijarnos en el fichero _activity_main.xml_:

```
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:orientation="vertical"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="match_parent"
        android:layout_height="0dp"
        android:layout_weight="2"
        android:text="@string/uno"
        android:textColor="@android:color/white"
        android:background="#B30000"/>

    <TextView
        android:layout_width="match_parent"
        android:layout_height="0dp"
        android:layout_weight="6"
        android:text="@string/dos"
        android:textColor="@android:color/white"
        android:background="#036200"/>

    <TextView
        android:layout_width="match_parent"
        android:layout_height="0dp"
        android:layout_weight="2"
        android:text="@string/tres"
        android:textColor="@android:color/white"
        android:background="#0362E0"/>

</LinearLayout>
```
Los textos de los _TextView_ se han insertado en el fichero _values/strings.xml_ y accedemos a ellos usando el símbolo @:

```
<resources>
    <string name="app_name">Ud2_Ejemplo6</string>
    <string name="uno">Uno</string>
    <string name="dos">Dos</string>
    <string name="tres">Tres</string>
</resources>
```

Tened en cuenta que si trabajamos en vertical el atributo _layout_height_ debe ser 0dp mientras que si lo hacemos en horizontal el atributo que debe ser 0dp es _layout_width_.
