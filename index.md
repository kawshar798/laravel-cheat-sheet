#laravel seeder

<p>#Create Seeder <pre>php artisan make:seeder UserSeeder</pre></p>
<p>#Exam  Seeder <pre> DB::table('users')->insert([
            'name' => Str::random(10),
            'email' => Str::random(10).'@gmail.com',
            'password' => Hash::make('password'),
        ]);</pre>
        </p>

<p>#Call  Seeders <pre>$this->call([
        UserSeeder::class
    ]);</pre></p>
    
    <p>#Run  Seeders <pre>php artisan db:seed
</pre>
</p>
    <p>#Run specific seeder<pre>php artisan db:seed --class=UserSeeder
</pre>
</p>
</p>
    <p># Fress  seeder<pre>php artisan migrate:fresh --seed
</pre>
</p>
