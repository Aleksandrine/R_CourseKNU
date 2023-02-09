#Task 1. Створити змінні базових (atomic) типів. Базові типи: character, numeric, integer, complex, logical.
character <- "Oleksandra"
numeric <- 7
integer <- 7L
complex <- 7i+7
logical <- TRUE

#Task 2. Створити вектори, які: містить послідовність з 5 до 75; містить числа 3.14, 2.71, 0, 13; 100 значень TRUE.
x1 <- 5:75
x2 <- c(3.14, 2.71, 0.13)
x3 <- rep(TRUE, 100)

#Task 3. Створити наступну матрицю за допомогою matrix, та за допомогою cbind або rbind
#MATRIX:
m1 <- matrix(c(0.5, 3.9, 0, 2, 1.3, 131, 2.2, 7, 3.5, 2.8, 4.6, 5.1),nrow = 4, ncol = 3)
m1

#RBIND:
a <- c(0.5, 1.3, 3.5)
b <- c(3.9, 131, 2.8)
c <- c(0, 2.2, 4.6)
d <- c(2, 7, 5.1)
m2 <- rbind(a,b,c,d)
m2

#CBIND:
a <- c(0.5, 3.9, 0, 2)
b <- c(1.3, 131, 2.2, 7)
c <- c(3.5, 2.8, 4.6, 5.1)
m3 <- cbind(a,b,c)
m3

#Task 4. Створити довільний список (list), в який включити всі базові типи.
list1 <- list("Oleksandra", 7, 7L, 7+7i, TRUE)
list1

#Task 5. Створити фактор з трьома рівнями «baby», «child», «adult».
fact1 <- factor(c("child", "adult", "baby", "child", "baby", "adult", "adult", "child", "baby", "baby", "adult"), levels = c("baby", "child", "adult"))
fact1

#Task 6. Знайти індекс першого значення NA в векторі 1, 2, 3, 4, NA, 6, 7, NA, 9, NA, 11. Знайти кількість значень NA.
task6 <- c(1, 2, 3, 4, NA, 6, 7, NA, 9, NA, 11)
task6_1NA <- min(which(is.na(task6)))
task6_1NA
count_NA <- length(which(is.na(task6)))
count_NA

#Task 7. Створити довільний data frame та вивести в консоль.
frame1 <- data.frame(Raiting = 1:4, Pets = c("Dog", "Cat", "Bird", "Monkey"))
frame1

#Task 8. Змінити імена стовпців цього data frame.
names(frame1) <- c("Rank", "Animal")
frame1


