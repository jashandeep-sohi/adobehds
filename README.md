adobehds
========

A PHP script to download Adobe HDS streams. Forked from K-S-V.

Usage
-----
```
$ php adobehds.php --help

KSV Adobe HDS Downloader

You can use script with following switches:                                    

 --help              displays this help                                        
 --debug             show debug output                                         
 --delete            delete fragments after processing                         
 --fproxy            force proxy for downloading of fragments                  
 --play              dump stream to stdout for piping to media player          
 --rename            rename fragments sequentially before processing           
 --version           display script version                                    
 --auth      [param] authentication string for fragment requests               
 --duration  [param] stop recording after specified number of seconds          
 --filesize  [param] split output file in chunks of specified size (MB)        
 --fragments [param] base filename for fragments                               
 --fixwindow [param] timestamp gap between frames to consider as timeshift     
 --manifest  [param] manifest file for downloading of fragments                
 --outdir    [param] destination folder for output file                        
 --outfile   [param] filename to use for output file                           
 --parallel  [param] number of fragments to download simultaneously            
 --proxy     [param] proxy for downloading of manifest                         
 --quality   [param] selected quality level (low|medium|high) or exact bitrate 
 --referrer  [param] Referer to use for emulation of browser requests          
 --start     [param] start from specified fragment                             
 --useragent [param] User-Agent to use for emulation of browser requests       
 --forwarded [param] Host name to forward for.
```

Added Features
--------------
In addition to the original features, this fork also supports the following features:

- Ability to specify `X-Forwarded-For` HTTP header. (--forwarded)


Removed Features
----------------

- Ability to update the script using the script. I consider it a security risk.
  (--update)
