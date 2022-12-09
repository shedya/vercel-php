# vercel-php

将php程序扔在主目录即可

![image](https://user-images.githubusercontent.com/53966497/206704861-8d211a82-2a87-4c54-8eb4-436d62dac0da.png)


#### vercel.json内容中

`{
  "functions": {
    "api/index.php": {
      "runtime": "vercel-php@0.5.2"
    }
  },
  "routes": [
    { "src": "/(.*)",  "dest": "/api/index.php" }
  ]
} 

对于的php本版为

- `vercel-php@0.5.2` - PHP 8.1.x
- `vercel-php@0.4.0` - PHP 8.0.x
- `vercel-php@0.3.2` - PHP 7.4.x

使用低于 "vercel-php@0.5.2" 版本可能会构建失败
