## 任务一：利用线性布局实现界面

​	关键代码：

```java
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal">

        <Button
            android:layout_width="80dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:layout_margin="4dp"

            android:text="One,One" />

        <Button
            android:layout_width="160dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:layout_margin="4dp"

            android:text="One,Two" />

        <Button
            android:layout_width="80dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:layout_margin="4dp"

            android:text="One,Three" />

        <Button
            android:layout_width="80dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:layout_margin="4dp"

            android:text="One,Four" />
    </LinearLayout>
```

​	实验截图：

![1](https//raw.githubusercontent.com/15305966258/twoapp/main/image/Snipaste_2022-10-04_10-18-34.png)

## 任务二：利用表格布局实现界面

关键代码：

```java
<TableRow
    android:layout_width="match_parent"
    android:layout_height="100dp">

    <TextView
        android:text="Open..."
        android:layout_weight="1"
        android:layout_height="wrap_content"
        android:layout_width="wrap_content"
        android:textSize="20dp"
        android:layout_marginLeft="10dp"
        />

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_weight="1"
        android:text="Ctrl-O"
        android:textAlignment="textEnd"
        android:layout_marginRight="10dp"
        android:textSize="20dp"/>

</TableRow>
```

实验截图：

![2](https//raw.githubusercontent.com/15305966258/twoapp/main/image/Snipaste_2022-10-04_10-18-54.png)

## 任务三：实现约束布局1

​	关键代码：

```java
<TextView
    android:id="@+id/textView23"
    android:layout_width="80dp"
    android:layout_height="30dp"
    android:layout_marginStart="16dp"
    android:layout_marginTop="44dp"
    android:background="#DADCDD"
    android:gravity="center"
    android:text="0"
    app:layout_constraintStart_toEndOf="@+id/textView20"
    app:layout_constraintTop_toBottomOf="@+id/textView17"
    tools:ignore="MissingConstraints" />

<TextView
    android:id="@+id/textView20"
    android:layout_width="80dp"
    android:layout_height="30dp"
    android:layout_marginStart="16dp"
    android:layout_marginTop="44dp"
    android:background="#DADCDD"
    android:gravity="center"
    android:text="."
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toBottomOf="@+id/textView14"
    tools:ignore="MissingConstraints" />

<TextView
    android:id="@+id/textView21"
    android:layout_width="80dp"
    android:layout_height="30dp"
    android:layout_marginTop="44dp"
    android:background="#DADCDD"
    android:gravity="center"
    android:text="-"
    app:layout_constraintEnd_toEndOf="parent"
    app:layout_constraintHorizontal_bias="0.742"
    app:layout_constraintStart_toEndOf="@+id/textView22"
    app:layout_constraintTop_toBottomOf="@+id/textView15"
    tools:ignore="MissingConstraints" />
```

实验截图：

![3](https//raw.githubusercontent.com/15305966258/twoapp/main/image/Snipaste_2022-10-04_10-22-44.png)

## 任务四：实现约束布局2

​	关键代码：

```java
<TextView
    android:id="@+id/textView13"
    android:layout_width="152dp"
    android:layout_height="125dp"
    android:background="#4CAF50"
    android:gravity="center"
    android:text="MARS"
    android:textColor="#FBFBFB"
    app:layout_constraintBottom_toBottomOf="parent"
    app:layout_constraintEnd_toEndOf="parent"
    app:layout_constraintHorizontal_bias="0.857"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toTopOf="parent"
    app:layout_constraintVertical_bias="0.188" />

<TextView
    android:id="@+id/textView12"
    android:layout_width="152dp"
    android:layout_height="125dp"
    android:background="#4CAF50"
    android:gravity="center"
    android:text="DCA"
    android:textColor="#FFFFFF"
    app:layout_constraintBottom_toBottomOf="parent"
    app:layout_constraintEnd_toEndOf="parent"
    app:layout_constraintHorizontal_bias="0.138"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toTopOf="parent"
    app:layout_constraintVertical_bias="0.188" />

<ImageView
    android:id="@+id/imageView"
    android:layout_width="88dp"
    android:layout_height="86dp"
    app:layout_constraintBottom_toBottomOf="parent"
    app:layout_constraintEnd_toEndOf="parent"
    app:layout_constraintHorizontal_bias="0.513"
    app:layout_constraintStart_toStartOf="parent"
    app:layout_constraintTop_toBottomOf="@+id/textView5"
    app:layout_constraintVertical_bias="0.091"
    app:srcCompat="@drawable/double_arrows" />
```

实验截图：

![4](https//raw.githubusercontent.com/15305966258/twoapp/main/image/Snipaste_2022-10-04_10-11-05.png)
