# Sonarr
PHP Wrapper for Sonarr https://sonarr.tv

Here is the Sonarr API Documentation that this package implements: https://github.com/Sonarr/Sonarr/wiki/API

## Example Usage
```php
use Kryptonit3\Sonarr\Sonarr;
```
```php
public function sonarrStatus()
{
    $sonarr = new Sonarr('http://127.0.0.1:8989', 'cf7544f71b6c4efcbb84b49011fc965c');
    
    return $this->sonarr->getSystemStatus();
}
```
### Output
```json
{  
   "version":"2.0.0.3732",
   "buildTime":"2016-01-16T16:22:08Z",
   "isDebug":false,
   "isProduction":true,
   "isAdmin":false,
   "isUserInteractive":false,
   "startupPath":"/volume1/@appstore/nzbdrone/share/NzbDrone",
   "appData":"/usr/local/nzbdrone/var/.config/NzbDrone",
   "osVersion":"3.10.35.0",
   "isMonoRuntime":true,
   "isMono":true,
   "isLinux":true,
   "isOsx":false,
   "isWindows":false,
   "branch":"master",
   "authentication":"basic",
   "sqliteVersion":"3.8.10.2",
   "urlBase":"",
   "runtimeVersion":"4.2.1 (Stable 4.2.1.102/6dd2d0d Mon Nov 30 14:47:31 CET 2015)"
}
```

For available methods reference included [Sonarr::class](src/Sonarr.php)
