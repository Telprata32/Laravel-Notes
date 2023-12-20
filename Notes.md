### You can put variables in your Controllers/Components

Like so:

```php
class DashBoardController extends Controller
{
   public function index(){

        $users = [
            [
                'name'=> 'Alex',
                'age'=>30,
            ],
            [
                'name'=>'John',
                'age'=>22,
            ]
        ];
   }

   return view('dashboard',[
        'users'=> $users
   ])
}
```

Notice the view function above has a second parameter; the view function can be used to send some data to the view like so:

```php
view('viewname', ['key' => $value])
```
