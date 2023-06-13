# Практическое задание 11.5

**CI** может использоваться не только в разработке программного обеспечения, но и при работе с данными.  

В качестве практики предлагаем вам настроить в любом из **CI-инструментов пайплайн**, выполняющий запрос к публичной базе данных проекта **rfam (rfam.org)**.

Проект занимается исследованием и хранением РНК (рибонуклеиновой кислоты).  
РНК — кислота, отвечающая за кодирование/декодирование и передачу в клетки данных, хранящихся в ДНК.

**Что необходимо сделать:**  

- Требуется настроить пайплайн, который будет запускаться при изменении SQL-скрипта, хранящегося в репозитории (его выбор также на ваше усмотрение).  

- Пайплайн должен запускать изменившийся скрипт и выводить результат запроса.  

## Решение  

Для решения задачи используется Gitlab-CI. При регистрации gitlab-runner в поле "Enter an executor" указываем "docker", а "image" пишем alpine:latest  
