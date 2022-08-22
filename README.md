            //1.获取模块的完整路径。 (E:\testnet\ConsoleApp1\ConsoleApp1\bin\Debug\net5.0\ConsoleApp1.exe)
            string path1 = System.Diagnostics.Process.GetCurrentProcess().MainModule.FileName;

            //2.获取和设置当前目录(该进程从中启动的目录)的完全限定目录 (E:\testnet\ConsoleApp1\ConsoleApp1\bin\Debug\net5.0)
            string path2 = System.Environment.CurrentDirectory;

            //3.获取应用程序的当前工作目录 (E:\testnet\ConsoleApp1\ConsoleApp1\bin\Debug\net5.0)
            string path3 = System.IO.Directory.GetCurrentDirectory();

            //4.获取程序的基目录 (E:\testnet\ConsoleApp1\ConsoleApp1\bin\Debug\net5.0\)
            string path4 = System.AppDomain.CurrentDomain.BaseDirectory;

            //5.获取和设置包括该应用程序的目录的名称  2、5一样。只是5返回的字符串后面多了一个"\"而已
            //(E:\testnet\ConsoleApp1\ConsoleApp1\bin\Debug\net5.0\)
            string path5 = System.AppDomain.CurrentDomain.SetupInformation.ApplicationBase;

            //就可以取得windows系统目录的路径
            //以下是一些常用的环境变量取值：
            var win1 = System.Environment.GetEnvironmentVariable("windir");
            var win2 = System.Environment.GetEnvironmentVariable("INCLUDE");
            var win3 = System.Environment.GetEnvironmentVariable("TMP");
            var win4 = System.Environment.GetEnvironmentVariable("TEMP");
            var win5 = System.Environment.GetEnvironmentVariable("Path");
            
            
            取消Token的一些实例运用
