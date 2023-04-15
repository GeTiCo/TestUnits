# UnitTest Work17 Файловая система

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

1. Комментарии Х
2. Рабочие тесты Х
