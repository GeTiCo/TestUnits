# UnitTest Work17 Файловая система

Информация о функциях

File.cs

    1. File - Конструктор, заполняюший информацию о файле
    2. GetSize - Возвращает размер файла
    3. GetFilename - Возвращает наименование файла

FileStorage.cs

    1. FileStorage - Конструктор принимающий размер файла
    2. FileStorage - Пустой конструктор
    3. Write - Запись файла и добавление в лист
    4. IsExists - Проверяет наличия файла
    5. Delete - Удаляет файл по имени
    6. GetFiles - Возвращает лист файлов
    7. GetFile - Возвращает файл по названию
    8. DeleteAllFiles - Удаляет все файлы

Изменения в Тестах

FileTest.cs

    Изменения параметров тестового класса
    
    1. Свойства из раздела ПРОВАЙДЕРЫ были переписаны на 'IEnumerable<object[]> NAME => new List<object[]>'

    Изменения в тестах
    
    1. Все методы тестов были переименованы на 'TestMethod, DynamicData(nameof(NAME))'

FileStorageTest.cs

    Изменения параметров тестового класса

    1. Константа 'public const string WRONG_SIZE_CONTENT_STRING' (Кол-во символов снижено до 200)
    2. Свойства из раздела ПРОВАЙДЕРЫ были переписаны на 'IEnumerable<object[]> NAME => new List<object[]>'
    3. В провайдере 'FilesForDeleteData' во 2 new object[] 1 параметр был заменен с 'null' на 'new File(TIC_TOC_TOE_STRING, CONTENT_STRING)'

    Изменения в тестах

    1. Все методы тестов были переименованы на 'TestMethod, DynamicData(nameof(NAME))'
    2. В тесте 'GetFileTest' Assert.IsFalse был заменен на Assert.IsTrue
    3. В тесте 'GetFilesTest' метод 'Test' был изменен на 'TestMethod'

1. Комментарии V
2. Рабочие тесты V
