# laravel55
git init
git add README.md
git commit -m "first commit"
git remote add origin https://github.com/wenhaiqing/laravel55.git
git push -u origin master

composer install
复制.env.example重新命名为.env
并复制一个key填入
php artisan migrate --seed
然后修改Illuminate/Foundation/Auth/AuthenticatesUsers.php 中的username()方法 把 email 改成 name
执行以上步骤就安装成功了


