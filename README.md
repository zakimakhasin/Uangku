Source Code Layout

# 1. Layout Tampilan Awal

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity"
    android:background="#D5D5D5">

    <TextView
        android:id="@+id/textView"
        android:layout_width="100dp"
        android:layout_height="30dp"
        android:text="UANGKU"
        android:textColor="@color/black"
        android:textSize="24dp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.083"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.022" />

    <ImageView
        android:id="@+id/imageView"
        android:layout_width="350dp"
        android:layout_height="230dp"
        android:src="@drawable/logo"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.491"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.359" />

    <TextView
        android:layout_width="250dp"
        android:layout_height="30dp"
        android:text="Selamat Datang di Uangku!"
        android:textSize="18dp"
        android:textStyle="bold"
        android:textColor="@color/black"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.186"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.617" />

    <Button
        android:id="@+id/btnLogin"
        android:layout_width="130dp"
        android:layout_height="48dp"
        android:background="@drawable/btn_bg"
        android:text="MASUK"
        android:textSize="14dp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.131"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.792" />

    <Button
        android:id="@+id/btnRegister"
        android:layout_width="130dp"
        android:layout_height="48dp"
        android:background="@drawable/btn_bg"
        android:text="DAFTAR"
        android:textSize="14dp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.889"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.792" />

    <TextView
        android:layout_width="350dp"
        android:layout_height="40dp"
        android:text="Dengan masuk atau mendaftar, kamu menyetujui Kebijakan Layanan dan Privasi"
        android:textSize="16dp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.606"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/btnRegister"
        app:layout_constraintVertical_bias="0.274" />

</androidx.constraintlayout.widget.ConstraintLayout>
```

# 2. Layout Tampilan Login

```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#D5D5D5">

    <androidx.cardview.widget.CardView
        android:id="@+id/login"
        android:layout_width="380dp"
        android:layout_height="wrap_content"
        android:layout_alignParentBottom="true"
        android:layout_marginBottom="120dp"
        app:cardCornerRadius="12dp"
        app:cardElevation="2dp"
        app:layout_constraintBottom_toTopOf="@+id/btnmasuk2"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent">

        <LinearLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:layout_margin="12dp"
            android:orientation="vertical">

            <TextView
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:text="Nomor Telepon*"
                android:textColor="@color/black"
                android:textSize="16dp"
                android:textStyle="bold" />

            <EditText
                android:id="@+id/editTextPhone"
                android:layout_width="match_parent"
                android:layout_height="40dp"
                android:layout_marginTop="5dp"
                android:background="@drawable/kolom"
                android:drawableStart="@drawable/ic_phone"
                android:drawableLeft="@drawable/ic_phone"
                android:ems="10"
                android:inputType="phone"
                tools:ignore="SpeakableTextPresentCheck" />

            <TextView
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:text="Bermasalah dengan nomer telepon?"
                android:textColor="#4287f5" />

            <TextView
                android:layout_width="wrap_content"
                android:layout_height="match_parent"
                android:layout_marginTop="10dp"
                android:text="Password"
                android:textColor="@color/black"
                android:textSize="16dp"
                android:textStyle="bold" />

            <EditText
                android:id="@+id/editTextTextPassword"
                android:layout_width="match_parent"
                android:layout_height="40dp"
                android:layout_marginTop="5dp"
                android:background="@drawable/kolom"
                android:drawableStart="@drawable/ic_lock"
                android:drawableLeft="@drawable/ic_lock"
                android:ems="10"
                android:inputType="textPassword"
                tools:ignore="SpeakableTextPresentCheck,SpeakableTextPresentCheck" />

        </LinearLayout>
    </androidx.cardview.widget.CardView>

    <TextView
        android:id="@+id/textView3"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginLeft="40dp"
        android:layout_marginBottom="90dp"
        android:text="*wajib"
        android:textColor="@color/black"
        app:layout_constraintBottom_toTopOf="@+id/btnmasuk2"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/login" />

    <Button
        android:id="@+id/btnmasuk2"
        android:layout_width="380dp"
        android:layout_height="40dp"
        android:layout_marginBottom="40dp"
        android:background="@drawable/btn_bg"
        android:text="Masuk"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent" />

    <ImageView
        android:id="@+id/logo"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        app:layout_constraintBottom_toTopOf="@+id/login"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.614"
        app:srcCompat="@drawable/logo" />

    <TextView
        android:id="@+id/textView4"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginBottom="5dp"
        android:text="Masukan Nomor yang terdaftar untuk masuk"
        app:layout_constraintBottom_toTopOf="@+id/login"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.121"
        app:layout_constraintStart_toStartOf="parent" />

    <ImageButton
        android:id="@+id/imageButton"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="16dp"
        app:layout_constraintEnd_toStartOf="@+id/textView5"
        app:layout_constraintHorizontal_bias="0.189"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:srcCompat="@drawable/ic_back" />

    <TextView
        android:id="@+id/textView5"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginEnd="148dp"
        android:text="Selamat Datang Kembali,"
        android:textColor="@color/black"
        android:textSize="18dp"
        android:textStyle="bold"
        app:layout_constraintBottom_toTopOf="@+id/logo"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.373" />
</androidx.constraintlayout.widget.ConstraintLayout>
```