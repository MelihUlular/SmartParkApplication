### Smart Park Application
Smart Park is an Android application that facilitates the management of car parking lots. Users can sign in, view available parking spots, and either fill or empty a parking lot spot.

## Features
- User Authentication: Users can sign up or sign in using their email and password.
- Parking Lot Management: Users can view the status of parking lots and fill or empty a parking spot.
- Realtime Database: Integration with Firebase Firestore to manage parking lot statuses in real-time.

## Dependencies
- Firebase Authentication
- Firebase Firestore
- Data Binding
- RecyclerView

### Code Structure
## MainActivity
Handles user authentication. If the user is already authenticated, they are redirected to the UserInterfaceActivity.

```Java
public class MainActivity extends AppCompatActivity {
    // Code for handling user sign in and sign up
}
```

## LotActivity
Manages the status of individual parking lot spots. Users can either fill or empty a parking spot.

```Java
public class LotActivity extends AppCompatActivity {
    // Code for managing parking lot status
}
```

## CarRecyclerViewAdapter
Adapter for displaying the parking lot spots in a RecyclerView. It listens for changes in the Firestore database to update the UI in real-time.

```Java
public class CarRecyclerViewAdapter extends RecyclerView.Adapter<CarRecyclerViewAdapter.CarHolder> {
    // Code for binding parking lot data to the RecyclerView
}
```

## ExampleUnitTest
Example unit test to verify the correctness of addition operations.

```Java
ublic class ExampleUnitTest {
    @Test
    public void addition_isCorrect() {
        assertEquals(4, 2 + 2);
    }
}
```

## ExampleInstrumentedTest
Instrumented test to verify the application context.

```Java
@RunWith(AndroidJUnit4.class)
public class ExampleInstrumentedTest {
    @Test
    public void useAppContext() {
        // Context of the app under test
        Context appContext = InstrumentationRegistry.getInstrumentation().getTargetContext();
        assertEquals("com.example.mobilecarapp", appContext.getPackageName());
    }
}
```

## Usage

- Sign Up: Create a new account using your email and password.
- Sign In: Log in with your credentials.
- View Parking Lots: See the status of various parking spots.
- Fill a Spot: If a spot is empty, fill it by clicking on it.
- Empty a Spot: If a spot is filled by you, you can empty it.
