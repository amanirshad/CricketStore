# CricketStore
A cricket scorecard maintaining android application 
<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@drawable/ball">

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:orientation="horizontal">

        <LinearLayout
            android:layout_width="0dp"
            android:layout_height="wrap_content"
            android:layout_weight="1"
            android:orientation="vertical"
            tools:context=".MainActivity">

            <TextView
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:fontFamily="sans-serif-medium"
                android:gravity="center_horizontal"
                android:padding="16dp"
                android:text="Team A"
                android:textColor="#616161"
                android:textSize="14sp" />

            <LinearLayout
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:orientation="horizontal">

                <TextView
                    android:id="@+id/team_a_runs"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:layout_weight="1"
                    android:fontFamily="sans-serif-light"
                    android:gravity="center_horizontal"
                    android:paddingBottom="24dp"
                    android:text="0"
                    android:textColor="#000000"
                    android:textSize="56sp" />

                <View
                    android:layout_width="1dp"
                    android:layout_height="match_parent"
                    android:layout_marginTop="8dp"
                    android:layout_marginBottom="8dp"
                    android:background="@android:color/holo_red_dark"></View>

                <TextView
                    android:id="@+id/team_a_wickets"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:layout_weight="1"
                    android:fontFamily="sans-serif-light"
                    android:gravity="center_horizontal"
                    android:paddingBottom="24dp"
                    android:text="0"
                    android:textColor="#000000"
                    android:textSize="56sp" />
            </LinearLayout>

            <LinearLayout
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_marginLeft="16dp"
                android:layout_marginRight="16dp"
                android:layout_marginBottom="16dp"
                android:orientation="horizontal">

                <TextView

                    android:layout_width="0dp"
                    android:layout_height="wrap_content"
                    android:layout_weight="2"
                    android:fontFamily="sans-serif-medium"
                    android:text="Overs:"
                    android:textSize="25sp" />

                <TextView
                    android:id="@+id/team_a_overs"
                    android:layout_width="0dp"
                    android:layout_height="wrap_content"
                    android:layout_weight="1"
                    android:fontFamily="sans-serif-medium"
                    android:text="0"
                    android:textSize="25sp"
                    android:textStyle="bold" />
            </LinearLayout>

            <Button

                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_marginLeft="24dp"
                android:layout_marginRight="24dp"
                android:layout_marginBottom="8dp"
                android:onClick="addSixForTeamA"
                android:text="+6 Runs" />

            <Button
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_marginLeft="24dp"
                android:layout_marginRight="24dp"
                android:layout_marginBottom="8dp"
                android:onClick="addFourForTeamA"
                android:text="+4 Runs" />

            <Button
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_marginLeft="24dp"
                android:layout_marginRight="24dp"
                android:layout_marginBottom="8dp"
                android:onClick="addThreeForTeamA"
                android:text="+3 Runs" />

            <Button
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_marginLeft="24dp"
                android:layout_marginRight="24dp"
                android:layout_marginBottom="8dp"
                android:onClick="addTwoForTeamA"
                android:text="+2 Runs" />

            <Button
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_marginLeft="24dp"
                android:layout_marginRight="24dp"
                android:layout_marginBottom="8dp"
                android:onClick="addOneForTeamA"
                android:text="+1 Runs" />

            <Button
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_marginLeft="24dp"
                android:layout_marginRight="24dp"
                android:layout_marginBottom="8dp"
                android:onClick="addWicketForTeamA"
                android:text="Wicket Down" />


        </LinearLayout>

        <View
            android:layout_width="1dp"
            android:layout_height="match_parent"
            android:layout_marginTop="16dp"
            android:background="@android:color/holo_red_dark"></View>

        <LinearLayout
            android:layout_width="0dp"
            android:layout_height="match_parent"
            android:layout_weight="1"
            android:orientation="vertical"
            tools:context=".MainActivity">

            <TextView
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:fontFamily="sans-serif-medium"
                android:gravity="center_horizontal"
                android:padding="16dp"
                android:text="Team B"
                android:textColor="#616161"
                android:textSize="14sp" />

            <LinearLayout
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:orientation="horizontal">

                <TextView
                    android:id="@+id/team_b_runs"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:layout_weight="1"
                    android:fontFamily="sans-serif-light"
                    android:gravity="center_horizontal"
                    android:paddingBottom="24dp"
                    android:text="0"
                    android:textColor="#000000"
                    android:textSize="56sp" />

                <View
                    android:layout_width="1dp"
                    android:layout_height="match_parent"
                    android:layout_marginTop="8dp"
                    android:layout_marginBottom="8dp"
                    android:background="@android:color/holo_red_dark"></View>

                <TextView
                    android:id="@+id/team_b_wickets"
                    android:layout_width="match_parent"
                    android:layout_height="wrap_content"
                    android:layout_weight="1"
                    android:fontFamily="sans-serif-light"
                    android:gravity="center_horizontal"
                    android:paddingBottom="24dp"
                    android:text="0"
                    android:textColor="#000000"
                    android:textSize="56sp" />
            </LinearLayout>

            <LinearLayout
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_marginLeft="16dp"
                android:layout_marginRight="16dp"
                android:layout_marginBottom="16dp"
                android:orientation="horizontal">

                <TextView
                    android:layout_width="0dp"
                    android:layout_height="wrap_content"
                    android:layout_weight="2"
                    android:fontFamily="sans-serif-medium"
                    android:text="Overs:"
                    android:textSize="25sp" />

                <TextView

                    android:id="@+id/team_b_overs"
                    android:layout_width="0dp"
                    android:layout_height="wrap_content"
                    android:layout_weight="1"
                    android:fontFamily="sans-serif-medium"
                    android:text="0"
                    android:textSize="25sp"
                    android:textStyle="bold" />
            </LinearLayout>

            <Button

                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_marginLeft="24dp"
                android:layout_marginRight="24dp"
                android:layout_marginBottom="8dp"
                android:onClick="addSixForTeamB"
                android:text="+6 Runs" />

            <Button
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_marginLeft="24dp"
                android:layout_marginRight="24dp"
                android:layout_marginBottom="8dp"
                android:onClick="addFourForTeamB"
                android:text="+4 Runs" />

            <Button
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_marginLeft="24dp"
                android:layout_marginRight="24dp"
                android:layout_marginBottom="8dp"
                android:onClick="addThreeForTeamB"
                android:text="+3 Runs" />

            <Button
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_marginLeft="24dp"
                android:layout_marginRight="24dp"
                android:layout_marginBottom="8dp"
                android:onClick="addTwoForTeamB"
                android:text="+2 Runs" />

            <Button
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_marginLeft="24dp"
                android:layout_marginRight="24dp"
                android:layout_marginBottom="8dp"
                android:onClick="addOneForTeamB"
                android:text="+1 Runs" />

            <Button
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_marginLeft="24dp"
                android:layout_marginRight="24dp"
                android:layout_marginBottom="8dp"
                android:onClick="addWicketForTeamB"
                android:text="Wicket Down" />


        </LinearLayout>

    </LinearLayout>

    <Button
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_alignParentBottom="true"
        android:layout_centerHorizontal="true"
        android:layout_marginBottom="32dp"
        android:onClick="resetScore"
        android:text="reset" />
</RelativeLayout>
