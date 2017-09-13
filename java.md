# Circularimage
import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        de.hdodenhof.circleimageview.CircleImageView firstimage = (de.hdodenhof.circleimageview.CircleImageView) findViewById(R.id.profile_image);

        int imageResource = getResources().getIdentifier("@drawable/tiger",null,this.getPackageName());
        firstimage.setImageResource(imageResource);

    }
}


