cmake_minimum_required(VERSION 3.27)
project(C__)

set(CMAKE_CXX_STANDARD 20)

set(BUILD_SHARED_LIBS FALSE)

include(FetchContent)
FetchContent_Declare(
        fmt
        GIT_REPOSITORY https://github.com/fmtlib/fmt
        GIT_TAG 10.2.1
)
FetchContent_Declare(
        SFML
        GIT_REPOSITORY https://github.com/SFML/SFML
        GIT_TAG 2.6.1
)
FetchContent_MakeAvailable(fmt)
FetchContent_MakeAvailable(SFML)


add_executable(Main lecture2/iterators/fast.cpp)
add_executable(WordReverse core/reversing_words.cpp)
add_executable(FmtPrinting core/fmt_printing.cpp)
add_executable(Cw2 lecture2/tasks_cw_v2/task.cpp)
add_executable(Lec3 lecture3/lecture3.cpp)
add_executable(Comp lecture3/comparators.cpp)
add_executable(Pred lecture3/lambdas_predicators.cpp)
add_executable(Tasks3 lecture3/task.cpp)
add_executable(abcde core/test.cpp)
add_executable(Read lecture4/workingFIles/readfile.cpp)
add_executable(Write lecture4/workingFIles/writefile.cpp)
add_executable(FileSys lecture4/workingFIles/filesystem.cpp)
add_executable(MostLines lecture4/workingFIles/main.cpp)
add_executable(Templ lecture4/templates/main.cpp)
add_executable(FileTasks lecture4/tasks/tasks.cpp)
add_executable(FileTasksA lecture4/tasks/analisys.cpp)
add_executable(Sudoku lecture4/tasks/sudoku.cpp)
add_executable(Replace lecture4/tasks/task4.cpp)
add_executable(Remove lecture4/tasks/task5.cpp)
add_executable(Six lecture4/task6/task6.cpp)
add_executable(SChunk core/lec4/chunk.cpp)
add_executable(ExtendA core/lec4/extend_algo.cpp)
add_executable(Backup core/lec4/backup.cpp)
add_executable(SFMLTest new/SFML/main.cpp)
add_executable(Lecture3 new/lecture3/wykład/main.cpp)
add_executable(Lecture5 new/lecture5/wykład/main.cpp)
add_executable(Lec5Task1 new/lecture5/tasks/task1.cpp)
add_executable(Anagrams core/lec5/anagrams.cpp)
add_executable(Cycle core/lec5/hasCycle.cpp)
add_executable(WordLengthGrouping core/lec5/word-legth.cpp)
add_executable(StudentNumbers core/lec5/student-numbers.cpp)
add_executable(TwoDPoints core/lec5/2d-points.cpp)
add_executable(Lecture6
        lecture6/headers/main.cpp
        lecture6/headers/utils/printer/printer.cpp
        lecture6/headers/utils/math/maths.cpp
        lecture6/headers/entity/point/point.cpp
)
#add_executable(TemplTest lecture6/templates/test.cpp)

add_executable(Lecture6_Templ lecture6/templates/main.cpp)
add_executable(Lecture6_Templ_2 lecture6/templates/main2.cpp)
add_executable(SFMP_TASK1 sfml_tasks/task1.cpp)
add_executable(SFML_TEST sfml_tasks/test/main.cpp sfml_tasks/test/Button/Button.cpp
        sfml_tasks/test/Point/Point.cpp)
add_executable(Lecture77 lecture7/task1.cpp)
add_executable(Core77 lecture7/core_.cpp)

target_link_libraries(Main fmt)
#target_link_libraries(TemplTest fmt)
target_link_libraries(WordReverse fmt)
target_link_libraries(FmtPrinting fmt)
target_link_libraries(Cw2 fmt)
target_link_libraries(Lec3 fmt)
target_link_libraries(Comp fmt)
target_link_libraries(Pred fmt)
target_link_libraries(Tasks3 fmt)
target_link_libraries(abcde fmt)
target_link_libraries(Read fmt)
target_link_libraries(Write fmt)
target_link_libraries(FileSys fmt)
target_link_libraries(MostLines fmt)
target_link_libraries(Templ fmt)
target_link_libraries(FileTasks fmt)
target_link_libraries(FileTasksA fmt)
target_link_libraries(Sudoku fmt)
target_link_libraries(Replace fmt)
target_link_libraries(Remove fmt)
target_link_libraries(Six fmt)
target_link_libraries(SChunk fmt)
target_link_libraries(ExtendA fmt)
target_link_libraries(Backup fmt)
target_link_libraries(SFMLTest sfml-graphics)
target_link_libraries(Lecture3 fmt)
target_link_libraries(Lecture5 fmt)
target_link_libraries(Lec5Task1 fmt)
target_link_libraries(Anagrams fmt)
target_link_libraries(Cycle fmt)
target_link_libraries(WordLengthGrouping fmt)
target_link_libraries(StudentNumbers fmt)
target_link_libraries(TwoDPoints fmt)
target_link_libraries(Lecture6 fmt)
target_link_libraries(Lecture6_Templ fmt)
target_link_libraries(Lecture6_Templ_2 fmt)
target_link_libraries(SFMP_TASK1 fmt sfml-graphics)
target_link_libraries(SFML_TEST fmt sfml-graphics)
target_link_libraries(Lecture77 fmt)
target_link_libraries(Core77 fmt)
