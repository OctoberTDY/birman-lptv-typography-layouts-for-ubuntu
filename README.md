# Currently WIP, nothing to see here
Todo: update install for 24.04, add no shift comma alternative version, update to Birman's 3.7.

# Типографская раскладка Ильи Бирмана для Ubuntu

Этот репозиторий содержит адаптацию русской и английской [типографской раскладки Ильи Бирмана](http://ilyabirman.ru/projects/typography-layout/) версии 3.4 для Ubuntu.

Раскладки протестированы в Ubuntu 18.04, 20.04. Версия для 16.04 доступна в одноимённом бранче.

![Снимок экрана](_keyboard/snapshot.png)

## Фичи раскладки

Эта раскладка позволяет вводить полезные символы, используя правый <kbd>Alt</kbd> (называемый AltGr). Например, чтобы получить знак евро **€**, вам нужно нажать <kbd>AltGr</kbd>+<kbd>У</kbd> в русском варианте или <kbd>AltGr</kbd>+<kbd>E</kbd> в английском. Дополнительный ряд символов доступен при нажатии еще и Shift-а, например <kbd>AltGr</kbd>+<kbd>С</kbd> даст знак копирайта **©**, а <kbd>AltGr</kbd>+<kbd>Shift</kbd>+<kbd>С</kbd> даст знак цента **¢**.

Как и оригинал, эта раскладка поддерживает ввод акцентов и ударений через «мёртвые клавиши», но процесс немного отличается от того, как это делается в Windows или на Маке. Например, для ввода буквы **ў**, нужно нажать и отпустить <kbd>AltGr</kbd>+<kbd>Shift</kbd>+<kbd>й</kbd>, а затем <kbd>у</kbd>.

## Установка

1. Скопируйте команду приведенную ниже, включая последний слэш:

    ```
    sudo apt-get -qq -y install wget && \
    wget -q -O /tmp/typo-birman-master.tar.gz https://github.com/vanushah/birman-typography-layouts-for-ubuntu/releases/download/v1.0/birman-typography-layouts-for-ubuntu-v1.0.tgz && \
    tar xf /tmp/typo-birman-master.tar.gz -C /tmp && \
    cd /tmp/birman-typography-layouts-for-ubuntu && \
    sudo /tmp/birman-typography-layouts-for-ubuntu/install.sh
    /
    ```

2. Откройте терминал (Ctrl+Alt+T), вставьте команду и нажмите клавишу Enter.

    Эта команда установит и включит обе раскладки в системе, активирует клавишу альтернативных символов (правый Alt), а также (опционально) установит переключение раскладок через Alt+Shift.

3. Дождитесь зелёного сообщения об успехе. В процессе установки может потребоваться ввод пароля.

4. **Обязательно перелогиньтесь после установки.**
