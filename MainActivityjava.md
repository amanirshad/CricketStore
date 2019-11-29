# CricketStore
A cricket scorecard maintaining android application 
package aman.irshad;

import androidx.appcompat.app.AppCompatActivity;
import android.os.Bundle;
import android.view.View;
import android.widget.TextView;

public class MainActivity extends AppCompatActivity {
    int teamARuns = 0;
    int teamAWickets = 0;
    int teamBRuns = 0;
    int teamBWickets = 0;
    int teamAOvers = 0;
    int teamBOvers = 0;
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
    }

    public void displayRunsForTeamA(int score){
        TextView runsView = (TextView) findViewById(R.id.team_a_runs);
        runsView.setText(String.valueOf(score));
    }
    public void displayRunsForTeamB(int score){
        TextView runsView = (TextView) findViewById(R.id.team_b_runs);
        runsView.setText(String.valueOf(score));
    }
    public void displayWicketsForTeamA(int wicket){
        TextView wicketsView = (TextView) findViewById(R.id.team_a_wickets);
        wicketsView.setText(String.valueOf(wicket));
    }
    public void displayWicketsForTeamB(int wicket){
        TextView wicketsView = (TextView) findViewById(R.id.team_b_wickets);
        wicketsView.setText(String.valueOf(wicket));
    }
    public void displayOversForTeamA(int overs){
        TextView oversView = (TextView) findViewById(R.id.team_a_overs);
        oversView.setText(String.valueOf(overs));
    }
    public void displayOversForTeamB(int overs){
        TextView oversView = (TextView) findViewById(R.id.team_b_overs);
        oversView.setText(String.valueOf(overs));
    }

    //reset everything
    public void resetScore(View view){
        teamARuns = 0;
        teamBRuns = 0;
        teamAWickets = 0;
        teamBWickets = 0;
        teamAOvers = 0;
        teamBOvers = 0;
        displayRunsForTeamA(teamARuns);
        displayRunsForTeamB(teamBRuns);
        displayWicketsForTeamA(teamAWickets);
        displayWicketsForTeamB(teamBWickets);
        displayOversForTeamA(teamAOvers);
        displayOversForTeamB(teamBOvers);
    }



    //For Team A
    public void addSixForTeamA(View view){
        teamARuns = teamARuns + 6;
        teamAOvers = teamAOvers + 1;
        displayOversForTeamA((teamAOvers/6));
        displayRunsForTeamA(teamARuns);

    }

    public void addFourForTeamA(View view){
        teamARuns = teamARuns + 4;
        displayRunsForTeamA(teamARuns);
        teamAOvers = teamAOvers + 1;
        displayOversForTeamA((teamAOvers/6));
    }

    public void addThreeForTeamA(View view){
        teamARuns = teamARuns + 3;
        displayRunsForTeamA(teamARuns);
        teamAOvers = teamAOvers + 1;
        displayOversForTeamA((teamAOvers/6));
    }

    public void addTwoForTeamA(View view){
        teamARuns = teamARuns + 2;
        displayRunsForTeamA(teamARuns);
        teamAOvers = teamAOvers + 1;
        displayOversForTeamA((teamAOvers/6));
    }

    public void addOneForTeamA(View view){
        teamARuns = teamARuns + 1;
        displayRunsForTeamA(teamARuns);
        teamAOvers = teamAOvers + 1;
        displayOversForTeamA((teamAOvers/6));
    }

    public void addWicketForTeamA(View view){
        teamAWickets = teamAWickets + 1;
        displayWicketsForTeamA(teamAWickets);
        teamAOvers = teamAOvers + 1;
        displayOversForTeamA((teamAOvers/6));
    }






    //For Team B
    public void addSixForTeamB(View view){
        teamBRuns = teamBRuns + 6;
        displayRunsForTeamB(teamBRuns);
        teamBOvers = teamBOvers + 1;
        displayOversForTeamB((teamBOvers/6));
    }
    public void addFourForTeamB(View view){
        teamBRuns = teamBRuns + 4;
        displayRunsForTeamB(teamBRuns);
        teamBOvers = teamBOvers + 1;
        displayOversForTeamB((teamBOvers/6));
    }
    public void addThreeForTeamB(View view){
        teamBRuns = teamBRuns + 3;
        displayRunsForTeamB(teamBRuns);
        teamBOvers = teamBOvers + 1;
        displayOversForTeamB((teamBOvers/6));
    }
    public void addTwoForTeamB(View view){
        teamBRuns = teamBRuns + 2;
        displayRunsForTeamB(teamBRuns);
        teamBOvers = teamBOvers + 1;
        displayOversForTeamB((teamBOvers/6));
    }
    public void addOneForTeamB(View view){
        teamBRuns = teamBRuns + 1;
        displayRunsForTeamB(teamBRuns);
        teamBOvers = teamBOvers + 1;
        displayOversForTeamB((teamBOvers/6));
    }
    public void addWicketForTeamB(View view){
        teamBWickets = teamBWickets + 1;
        displayWicketsForTeamB(teamBWickets);
        teamBOvers = teamBOvers + 1;
        displayOversForTeamB((teamBOvers/6));
    }


}
