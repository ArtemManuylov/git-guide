## Установка Git и Git Bash для Windows

Перед началом работы необходимо установить Git, который включает в себя Git Bash — эмулятор командной строки для работы с Git.

### Инструкция по установке

1. **Скачайте установочный файл с официального сайта.**
   
    Перейдите на [официальный сайт Git](https://git-scm.com/). Нажмите на кнопку **Download for Windows**. Будет скачан установочный файл.

2. **Запустите установочный файл.**
   
   Дважды щелкните по скачанному файлу. Появится окно контроля учетных записей. Нажмите «Да», чтобы разрешить приложению вносить изменения.

3. **Настройте параметры установки.**

    Следуйте шагам мастера установки. Рекомендуется оставить настройки по умолчанию, но на некоторых шагах стоит обратить внимание:
    * **Select Components:**
     
      Оставьте все галочки по умолчанию. Убедитесь, что `Git Bash` и `Git GUI` выбраны.
  
      ![Select Components](../../images/SelectComponents.png)

    * **Choosing the default editor:**
      Если вы планируете писать код в **VSCode**, выберите **Visual Studio Code** из выпадающего списка. Если вы не уверены, оставьте **Vim**.
  
      ![Default Editor](../../images/DefaultEditor.png)

      > *Вы всегда можете изменить редактор позже с помощью команды*:`git config --global core.editor "code --wait"`.

    * **Adjusting the name of the initial branch in new repositories:** 
     
      Раньше Git по умолчанию создавал начальную ветку с именем `master`. Однако сейчас сообщество переходит на использование нейтрального имени `main`.
     
      Выберите: `Override the default branch name` — задать свое имя `main`.

      ![Adjusting the name of the initial branch in new repositories](../../images/NameBranch.png)

    * **Adjusting your PATH environment:** 
     
      Выберите: `Git from the command line and also from 3rd-party software` — это самый гибкий вариант, позволяющий использовать Git в любом терминале.
  
      ![Adjusting your PATH environment](../../images/AdjustingEnvironme.png)

    * **Choosing the SSH executable:** 
     
      Git предложит выбрать, какой SSH-клиент использовать для работы с репозиториями по протоколу SSH. 
     
      SSH (Secure Shell) — это протокол для безопасного подключения к удаленным серверам.
     
       Выберите: `Use external OpenSSH` — стандартный OpenSSH, который идет в комплекте с Git для Windows
  
      ![Choosing the SSH executable](../../images/ssh.png)

    * **Choosing HTTPS transport backend:** 
      
      Git предложит выбрать бэкенд для HTTPS-соединений. Этот выбор влияет на то, как Git будет работать с защищенными репозиториями на GitHub и других хостингах.

      Оставьте галочки по умолчанию: `Use the OpenSSL library`.
    * **Configuring the line ending conversions:**
     
      Это важный пункт для совместимости между Windows и Linux/macOS. 
      
      Выберите: `Checkout Windows-style, commit Unix-style line endings`.

      ![Configuring the line ending conversions](../../images/Configuring.png)

    * **Configuring the terminal emulator to use with git bash:** 
     
     Git предложит выбрать эмулятор терминала для работы с Git Bash. Этот выбор влияет на то, как будет выглядеть и работать ваша командная строка.
     
      Выберите: `Use MinTTY (the default terminal of MSYS2)` — более привычный интерфейс для пользователей UNIX-подобных систем (Linux, macOS).
  
      ![Configuring the terminal emulator to use with git bash](../../images/ConfiguringEmulator.png)

    * **Choose the default behavior of git pull:**
    
      Git предложит выбрать стратегию по умолчанию для команды `git pull`. Этот выбор влияет на то, как Git будет объединять изменения из удаленного репозитория с вашей локальной веткой.
     
      Оставьте галочки по умолчанию: `Fast-forward or merge` — это безопасный вариант, который гарантирует сохранность ваших данных и создает понятную историю коммитов.
    * **Choose a credential helper:** 
     
      Git предложит выбрать способ хранения ваших учетных данных для автоматической аутентификации на GitHub и других хостингах.

      Оставьте галочки по умолчанию: `Git Credential Manager` — надежно сохраняет ваши данные для входа и избавляет от рутинного ввода пароля при каждой операции с GitHub. 

    * **Configuring extra options:**
  
      Git предложит несколько дополнительных опций, которые расширяют функциональность и улучшают производительность.
      
      Оставьте галочки по умолчанию: `Enable file system caching` — эта опция значительно ускоряет работу Git с большими репозиториями.

4. **Завершите установку**

   Нажмите `Install` и дождитесь окончания процесса. После этого нажмите `Finish`.