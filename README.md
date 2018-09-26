# Grading-System-App
# This small Androind application helps students to calculate their grades by entering the total marks they received in a course. 


# The XML and Java codes used in this application can be found below. 

# XML codes:
<?xml version="1.0" encoding="utf-8"?>
<android.support.constraint.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity"
    tools:layout_editor_absoluteY="81dp">

    <TextView
        android:id="@+id/textView"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:layout_marginBottom="18dp"
        android:layout_marginEnd="27dp"
        android:layout_marginLeft="27dp"
        android:layout_marginRight="27dp"
        android:layout_marginStart="27dp"
        android:layout_marginTop="19dp"
        android:text="Student Grading System"
        android:textColor="@android:color/black"
        android:textSize="30sp"
        app:layout_constraintBottom_toTopOf="@+id/studetnid"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/textView2"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:layout_marginBottom="187dp"
        android:layout_marginEnd="26dp"
        android:layout_marginLeft="16dp"
        android:layout_marginRight="26dp"
        android:layout_marginStart="16dp"
        android:layout_marginTop="76dp"
        android:text="Student ID"
        android:textSize="24sp"
        app:layout_constraintBottom_toTopOf="@+id/idTextView"
        app:layout_constraintEnd_toStartOf="@+id/studetnid"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <TextView
        android:id="@+id/textView3"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:layout_marginBottom="10dp"
        android:layout_marginEnd="20dp"
        android:layout_marginLeft="16dp"
        android:layout_marginRight="20dp"
        android:layout_marginStart="16dp"
        android:text="Course Code"
        android:textSize="24sp"
        app:layout_constraintBottom_toTopOf="@+id/textView4"
        app:layout_constraintEnd_toStartOf="@+id/coursecode"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/studetnid" />

    <TextView
        android:id="@+id/textView4"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:layout_marginBottom="10dp"
        android:layout_marginEnd="20dp"
        android:layout_marginLeft="16dp"
        android:layout_marginRight="20dp"
        android:layout_marginStart="16dp"
        android:text="Total Marks"
        android:textSize="24sp"
        app:layout_constraintBottom_toTopOf="@+id/button"
        app:layout_constraintEnd_toStartOf="@+id/marks"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/textView3" />

    <EditText
        android:id="@+id/studetnid"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:layout_marginBottom="9dp"
        android:layout_marginEnd="50dp"
        android:layout_marginRight="50dp"
        android:ems="10"
        android:hint="Enter your ID"
        android:inputType="number"
        android:textSize="18sp"
        app:layout_constraintBottom_toTopOf="@+id/textView3"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toEndOf="@+id/textView2"
        app:layout_constraintTop_toBottomOf="@+id/textView" />

    <EditText
        android:id="@+id/coursecode"
        android:layout_width="0dp"
        android:layout_height="42dp"
        android:layout_marginBottom="50dp"
        android:layout_marginEnd="44dp"
        android:layout_marginRight="44dp"
        android:layout_marginTop="52dp"
        android:ems="10"
        android:hint="Enter course code"
        android:inputType="textCapCharacters"
        app:layout_constraintBottom_toBottomOf="@+id/marks"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toEndOf="@+id/textView3"
        app:layout_constraintTop_toTopOf="@+id/studetnid" />

    <EditText
        android:id="@+id/marks"
        android:layout_width="0dp"
        android:layout_height="wrap_content"
        android:layout_marginBottom="5dp"
        android:layout_marginEnd="44dp"
        android:layout_marginRight="44dp"
        android:ems="10"
        android:hint="Enter your Marks"
        android:inputType="number|numberDecimal"
        app:layout_constraintBottom_toTopOf="@+id/button"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toEndOf="@+id/textView4" />

    <Button
        android:id="@+id/button"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginBottom="26dp"
        android:layout_marginEnd="10dp"
        android:layout_marginRight="10dp"
        android:text="SHOW GRADE"
        app:layout_constraintBottom_toTopOf="@+id/studentidshow"
        app:layout_constraintEnd_toEndOf="@+id/studentidshow"
        app:layout_constraintTop_toBottomOf="@+id/textView4" />

    <TextView
        android:id="@+id/idTextView"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:layout_marginBottom="10dp"
        android:layout_marginEnd="47dp"
        android:layout_marginLeft="16dp"
        android:layout_marginRight="47dp"
        android:layout_marginStart="16dp"
        android:textSize="18sp"
        app:layout_constraintBottom_toTopOf="@+id/codeTextView"
        app:layout_constraintEnd_toStartOf="@+id/studentidshow"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/textView2" />

    <TextView
        android:id="@+id/codeTextView"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:layout_marginBottom="14dp"
        android:layout_marginEnd="42dp"
        android:layout_marginLeft="16dp"
        android:layout_marginRight="42dp"
        android:layout_marginStart="16dp"
        android:textSize="18sp"
        app:layout_constraintBottom_toTopOf="@+id/markTextView"
        app:layout_constraintEnd_toStartOf="@+id/coursecodeshow"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/idTextView" />

    <TextView
        android:id="@+id/markTextView"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:layout_marginBottom="19dp"
        android:layout_marginEnd="42dp"
        android:layout_marginLeft="16dp"
        android:layout_marginRight="42dp"
        android:layout_marginStart="16dp"
        android:textSize="18sp"
        app:layout_constraintBottom_toTopOf="@+id/gradeTextView"
        app:layout_constraintEnd_toStartOf="@+id/marksshow"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/codeTextView" />

    <TextView
        android:id="@+id/gradeTextView"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:layout_marginBottom="10dp"
        android:layout_marginEnd="37dp"
        android:layout_marginLeft="27dp"
        android:layout_marginRight="37dp"
        android:layout_marginStart="27dp"
        android:textSize="18sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toStartOf="@+id/grade"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/markTextView" />

    <TextView
        android:id="@+id/studentidshow"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:layout_marginBottom="10dp"
        android:layout_marginEnd="123dp"
        android:layout_marginRight="123dp"
        android:textColor="@android:color/black"
        app:layout_constraintBottom_toTopOf="@+id/coursecodeshow"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toEndOf="@+id/idTextView"
        app:layout_constraintTop_toBottomOf="@+id/button" />

    <TextView
        android:id="@+id/coursecodeshow"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:layout_marginBottom="11dp"
        android:layout_marginEnd="118dp"
        android:layout_marginRight="118dp"
        android:textColor="@android:color/black"
        app:layout_constraintBottom_toTopOf="@+id/marksshow"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toEndOf="@+id/codeTextView"
        app:layout_constraintTop_toBottomOf="@+id/studentidshow" />

    <TextView
        android:id="@+id/marksshow"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:layout_marginBottom="16dp"
        android:layout_marginEnd="118dp"
        android:layout_marginRight="118dp"
        android:textColor="@android:color/black"
        app:layout_constraintBottom_toTopOf="@+id/grade"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toEndOf="@+id/markTextView"
        app:layout_constraintTop_toBottomOf="@+id/coursecodeshow" />

    <TextView
        android:id="@+id/grade"
        android:layout_width="0dp"
        android:layout_height="0dp"
        android:layout_marginBottom="7dp"
        android:layout_marginEnd="124dp"
        android:layout_marginRight="124dp"
        android:textColor="@android:color/holo_green_dark"
        android:textSize="18sp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toEndOf="@+id/gradeTextView"
        app:layout_constraintTop_toBottomOf="@+id/marksshow" />
</android.support.constraint.ConstraintLayout>



 

# Java codes:
package com.example.itcs.gradeapplication;

import android.os.Bundle;
import android.support.v7.app.AppCompatActivity;
import android.view.View;
import android.widget.Button;
import android.widget.EditText;
import android.widget.TextView;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        Button calcbutton = (Button) findViewById(R.id.button);
        calcbutton.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {

                EditText id = (EditText) findViewById(R.id.studetnid);
                EditText code = (EditText) findViewById(R.id.coursecode);
                EditText mark = (EditText) findViewById(R.id.marks);
                TextView idshow = (TextView) findViewById(R.id.studentidshow);
                TextView codeshow = (TextView) findViewById(R.id.coursecodeshow);
                TextView markshow= (TextView) findViewById(R.id.marksshow);
                TextView gradeshow = (TextView) findViewById(R.id.grade);
                TextView idtextview = (TextView) findViewById(R.id.idTextView);
                TextView codetextview = (TextView) findViewById(R.id.codeTextView);
                TextView marktextview = (TextView) findViewById(R.id.markTextView);
                TextView gradetextview = (TextView) findViewById(R.id.gradeTextView);



                int studentid = Integer.parseInt(id.getText().toString());
                String codeid = code.getText().toString();
                float studentmark = Float.parseFloat(mark.getText().toString());


                idshow.setText(studentid + "");
                codeshow.setText(codeid + "");
                markshow.setText(studentmark + "");
                idtextview.setText("Student ID: ");
                codetextview.setText("Course ID: ");
                marktextview.setText("Total Marks: ");
                gradetextview.setText("Grade: ");

                if (studentmark >= 94) {
                    gradeshow.setText("A");
                }
                else if (studentmark >= 90) {
                    gradeshow.setText("A-");
                }
                else if (studentmark >= 87) {
                    gradeshow.setText("B+");
                }
                else if (studentmark >= 84) {
                    gradeshow.setText("B");
                }
                else if (studentmark >= 80) {
                    gradeshow.setText("B-");
                }
                else if (studentmark >= 77) {
                    gradeshow.setText("C+");
                }
                else if (studentmark >= 74) {
                    gradeshow.setText("C");
                }
                else if (studentmark >= 70) {
                    gradeshow.setText("C-");
                }
                else if (studentmark >= 67) {
                    gradeshow.setText("D+");
                }
                else if (studentmark >= 60) {
                    gradeshow.setText("D");
                }
                else  {
                    gradeshow.setText("F");
                }

            }
        });
    }
}

