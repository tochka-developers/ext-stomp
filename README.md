stomp
=====

В файле stopm.c закоментирован код:
```
if (frame->body_length > 0) {
    smart_str_appendl(&buf, "content-length:", sizeof("content-length:") - 1);
    smart_str_append_long(&buf, frame->body_length);
    smart_str_appendc(&buf, '\n');
}
```

Изменена версия расширения