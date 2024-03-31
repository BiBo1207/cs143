## Reference Material

- [bilibili](https://www.bilibili.com/video/BV1cE411f78c/?spm_id_from=333.337.search-card.all.click&vd_source=b3a0dc5b9cad4d6e651c7182a9be42a3)

- [edx](https://learning.edx.org/course/course-v1:StanfordOnline+SOE.YCSCS1+2T2020/home)

- [知乎](https://zhuanlan.zhihu.com/p/226190284)

- You can download assignments without answers from the `skeleton` branch.
## Dev Environment Configuration
All assignments are based on the Ubuntu 20.04.  
- `sudo apt-get install bison build-essential csh libxaw7-dev` 
   
- Install [flex-2.5.35](https://src.fedoraproject.org/lookaside/pkgs/flex/flex-2.5.35.tar.bz2/10714e50cea54dc7a227e3eddcd44d57/). Once downloaded and unzipped, execute the commands:   
    ```shell
        cd ./flex-2.5.35/
        ./configure && make && sudo make install
    ```   
    If you encounter the error `GNU M4 1.4 is required`, you can search for solutions in [M4](http://ftp.gnu.org/gnu/m4).   
- Add the `bin` folder located within the repo to your system's `PATH` environment variable.   
- Test your dev environment:   
    ```shell
        # Go to the <your repo path>/assignments/PA1 folder
        make test
    ```
    If the environment is configured successfully, you will see the following message in your terminal:
    ```
        Nothing implemented
        COOL program successfully executed
    ```
    And, if you encounter an error similar to `'.../.i686/spim: No such file or directory'`, installing `libc6-i386` might be a solution to try.
    ```txt
        sudo apt-get install libc6-i386
    ```
## Acknowledgements
- [anarion](https://zhuanlan.zhihu.com/p/226190284)
- [simviso官方](https://space.bilibili.com/2494318)