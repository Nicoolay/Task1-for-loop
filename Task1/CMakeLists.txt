#����������� ������ cmake
cmake_minimum_required(VERSION 3.10)
#��� �������
project(demoVendorCatch2)
#��������� �������������, � ������� ����� catch2
add_subdirectory(catch2)
#��������� ���� - ����������, � �������� �������� � ������������ �����������
add_executable(${PROJECT_NAME} Task1.cpp)
#��������� � catch2, � ������� ��� ���� main
target_link_libraries(${PROJECT_NAME} PRIVATE Catch2::Catch2 Catch2::Catch2WithMain)