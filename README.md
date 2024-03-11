# Conda Installation and User Guide / Conda Kurulum ve Kullanım Kılavuzu

### Installing Anaconda in the Home Directory / Anaconda'yı Ana Dizine Kurma
##### Download miniconda / Miniconda'yı İndirme: 

```
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh
``` 

###### You can delete the script after it is finished / İşlem tamamlandıktan sonra script'i silebilirsiniz:

```
rm Miniconda3-latest-Linux-x86_64.sh
```

###### Update Conda / Conda Güncelleme:

```
eval "$(miniconda3/bin/conda shell.bash hook)"
```

##### Create Environment With Conda / Conda ile Ortam Oluşturma:

###### Named Your Env / Oluşturulmak İstenen Ortamı İsimlendiriniz.

```
conda create -n deneme
```

###### Switch Env / Env Geçişi;

```
conda activate deneme
```
###### Turn Main Env / Ana Ortama Dönme:
```
conda deactivate
```

##### İnstall Packages With Conda / Conda ile Paket Yükleme:

```
conda install -c bioconda fastqc
```
###### "-c --channel"
Choose channel with command "-c" / "-c" komutu ile kanal seçilir.

### Some Conda Options and Commands / Bazı Conda Seçenekleri ve Komutları

#### Options / Seçenekler:

``` -h, --help ```         
##### (EN) Show help message 
##### (TR) Yardım mesajını gösterir.
``` -v, --verbose ```      
##### (EN) Can be used multiple times. Once for detailed output, twice for INFO logging, thrice for DEBUG logging, four times for TRACE logging.
##### (TR) Çok kez kullanılabilir. Bir kez ayrıntılı çıktı için, iki kez INFO günlüğü için, üç kez DEBUG günlüğü için, dört kez TRACE günlüğü için. Bu ifade genellikle bir programın çıktısının detay seviyesini belirlemek için kullanılır. Daha fazla detay istendikçe, ifade daha çok kez kullanılır. Örneğin, TRACE günlüğü en ayrıntılı günlük seviyesidir ve bu nedenle ifade dört kez kullanılır. Bu, genellikle hata ayıklama ve sorun giderme durumlarında kullanışlıdır.
``` --no-plugins ```       
##### (EN) Disable all plugins that are not built into conda.
##### (TR) Conda’ya dahili olarak eklenmeyen tüm eklentileri devre dışı bırakın.
``` -V, --version ```      
##### (EN) Show the conda version number. 
##### (TR) Conda version numarasını gösterir.

  #### Commands / Komutlar: 

``` activate ```         
##### (EN) Activate a conda environment.
##### (TR) Conda ortamını aktive eder.
``` clean ```            
##### (EN) Remove unused packages and caches.
##### (TR) Kullanılmayan paket ve önbelleği temizler.
``` compare ```          
##### (EN) Compare packages between conda environments.
##### (TR) Conda ortamları arasında paketleri karşılaştırın.
``` config ```         
##### (EN) Modify configuration values in .condarc.
##### (TR) .condarc'daki yapılandırma değerlerini değiştirin.
###### (EN) In this case, the “.condarc” file is a configuration file for ‘conda’, a package manager and environment manager. This file is used by advanced users to configure various aspects of ‘conda’. This is usually useful in debugging and troubleshooting situations. For example, you can set configuration options by directly editing the ‘.condarc’ file or using the ‘conda config --set’ command.
###### (TR) Bu durumda, “.condarc” dosyası, ‘conda’ adlı bir paket yöneticisi ve ortam yöneticisinin yapılandırma dosyasıdır. Bu dosya, 'conda’nın çeşitli yönlerini yapılandırmak için gelişmiş kullanıcılar tarafından kullanılır. Bu, genellikle hata ayıklama ve sorun giderme durumlarında kullanışlıdır. Örneğin, ‘.condarc’ dosyasını doğrudan düzenleyerek veya ‘conda config --set’ komutunu kullanarak yapılandırma seçeneklerini ayarlayabilirsiniz.
``` content-trust ```  
##### (EN) Signing and verification tools for Conda
##### (TR) Conda için imzalama ve doğrulama araçları 
###### (EN) In this case, we are talking about signing and verification tools for ‘conda’, a package manager and environment manager. These tools are designed to allow users who obtain a package or data about that package in the ‘conda’ ecosystem to know whether this data is reliable (for example, it comes from a trusted source and has not been tampered with). It also includes a core library and a core CLI (Command Line Interface) that provides signing, verification, and trust delegation functionality.
###### (TR) Bu durumda, ‘conda’ adlı bir paket yöneticisi ve ortam yöneticisi için imzalama ve doğrulama araçlarından bahsediliyor. Bu araçlar, ‘conda’ ekosisteminde bir paket veya o paket hakkındaki verileri elde eden kullanıcıların, bu verilerin güvenilir olup olmadığını (örneğin, güvenilir bir kaynaktan geliyor ve üzerinde oynanmamış) bilebilmelerini sağlamak için tasarlanmıştır. Ayrıca, imzalama, doğrulama ve güven delegasyonu işlevselliği sağlayan temel bir kütüphane ve temel bir CLI (Komut Satırı Arayüzü) içerir.
``` create ```         
##### (EN) Create a new conda environment from a list of specified packages.
##### (TR) Belirtilen paketlerin listesinden yeni bir conda ortamı oluşturun.
``` deactivate ```     
##### (EN) Deactivate the current active conda environment.
##### (TR) Geçerli aktif conda ortamını devre dışı bırakın.
``` doctor ```         
##### (EN) Display a health report for your environment.
##### (TR) Ortamın sağlık raporunu gösterir.
``` env ```            
##### (EN) See `conda env --help`.
##### (TR) `conda env --help` 'yı görün.
``` info ```          
##### (EN) Display information about current conda install.
##### (TR) Geçerli conda kurulumu hakkında bilgi gösterir.
``` init ```           
##### (EN) Initialize conda for shell interaction.
##### (TR) Conda'yı shell etkileşimi için başlatın.
###### (EN) In this case, you want to initiate shell interaction for ‘conda’, a package manager and environment manager. This is usually useful in debugging and troubleshooting situations. For example, you can start 'conda’s interaction with the shell by using the ‘conda init’ command.
###### (TR) Bu durumda, ‘conda’ adlı bir paket yöneticisi ve ortam yöneticisi için shell etkileşimini başlatmak istenmektedir. Bu, genellikle hata ayıklama ve sorun giderme durumlarında kullanışlıdır. Örneğin, ‘conda init’ komutunu kullanarak 'conda’nın kabukla etkileşimini başlatabilirsiniz.
``` install ```        
##### (EN) Install a list of packages into a specified conda environment.
##### (TR) Belirtilen bir conda ortamına paket listesini yükleyin.
``` list ```           
##### (EN) List installed packages in a conda environment.
##### (TR) Conda otamındaki yüklü paketleri listeleyin.
``` notices ```        
##### (EN) Retrieve latest channel notifications.
##### (TR) En son kanal bildirimlerini alın.
``` package ```         
##### (EN) Create low-level conda packages. (EXPERIMENTAL)
##### (TR) Düşük seviye conda paketlerini oluşturun. (DENEYSEL)
###### (EN) In this case, you want to create low-level packages for ‘conda’, a package manager and environment manager. This is usually useful in debugging and troubleshooting situations. For example, you can create low-level ‘conda’ packages using the ‘conda package’ command. However, as this feature is still experimental, it is recommended to be careful when using it.
###### (TR) Bu durumda, ‘conda’ adlı bir paket yöneticisi ve ortam yöneticisi için düşük seviye paketlerin oluşturulması istenmektedir. Bu, genellikle hata ayıklama ve sorun giderme durumlarında kullanışlıdır. Örneğin, ‘conda package’ komutunu kullanarak düşük seviye ‘conda’ paketleri oluşturabilirsiniz. Ancak, bu özellik hala deneysel olduğu için, kullanırken dikkatli olmanız önerilir.
``` remove (uninstall) ```
##### (EN) Remove a list of packages from a specified conda environment.
##### (TR) Belirtilen bir conda ortamından paket listesini kaldırın.
``` rename ```         
##### (EN) Rename an existing environment.
##### (TR) Mevcut bir ortamı yeniden adlandırın.
``` repoquery ```      
##### (EN) Advanced search for repodata.
##### (TR) Repodata için gelişmiş arama
###### (EN) In this case, ‘repodata’ usually refers to a dataset containing package metadata for ‘conda’, a package manager and environment manager. This is usually useful in debugging and troubleshooting situations. For example, you can perform advanced searches in ‘repodata’ using the ‘conda search --info’ command.
###### (TR) Bu durumda, ‘repodata’ genellikle bir paket yöneticisi ve ortam yöneticisi olan ‘conda’ için paket meta verilerini içeren bir veri setini ifade eder. Bu, genellikle hata ayıklama ve sorun giderme durumlarında kullanışlıdır. Örneğin, ‘conda search --info’ komutunu kullanarak ‘repodata’ içinde gelişmiş aramalar yapabilirsiniz.
``` run ```            
##### (EN) Run an executable in a conda environment.
##### (TR) Conda ortamında bir yürütülebilir dosya çalıştırın.
###### (EN) In this case, you want to run a specific executable file in a specific environment for ‘conda’, a package manager and environment manager. This is usually useful in debugging and troubleshooting situations. For example, you can run a specific executable file in a specific ‘conda’ environment using the ‘conda run’ command.
###### (TR) Bu durumda, ‘conda’ adlı bir paket yöneticisi ve ortam yöneticisi için belirli bir ortamda belirli bir yürütülebilir dosyanın çalıştırılması istenmektedir. Bu, genellikle hata ayıklama ve sorun giderme durumlarında kullanışlıdır. Örneğin, ‘conda run’ komutunu kullanarak belirli bir ‘conda’ ortamında belirli bir yürütülebilir dosyayı çalıştırabilirsiniz.
``` search ```         
##### (EN) Search for packages and display associated information using the MatchSpec format.
##### (TR) MatchSpec formatını kullanarak paketleri arayın ve ilişkili bilgileri görüntüleyin.
###### (EN) In this case, you want to search for packages and display related information using the MatchSpec format for ‘conda’, a package manager and environment manager. This is usually useful in debugging and troubleshooting situations. For example, you can search for packages and display related information using the MatchSpec format with the ‘conda search’ command.
###### (TR) Bu durumda, ‘conda’ adlı bir paket yöneticisi ve ortam yöneticisi için MatchSpec formatını kullanarak paketlerin aranması ve ilişkili bilgilerin görüntülenmesi istenmektedir. Bu, genellikle hata ayıklama ve sorun giderme durumlarında kullanışlıdır. Örneğin, ‘conda search’ komutunu kullanarak MatchSpec formatını kullanarak paketleri arayabilir ve ilişkili bilgileri görüntüleyebilirsiniz.
``` update (upgrade) ```
##### (EN) Update conda packages to the latest compatible version.
##### (TR) Conda paketlerini en son uyumlu sürüme güncelleyin.