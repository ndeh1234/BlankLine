# BlankLine
def show_read_books():
    read_books = store.get_books_by_read_value(True)
    print("\n")  # adding blank line before list of books
    ui.show_books(read_books)
    print("\n")  # adding blank line before list of books


def show_unread_books():
    unread_books = store.get_books_by_read_value(False)
    print("\n")  # adding blank line before list of books
    ui.show_books(unread_books)
    print("\n")  # adding blank line before list of books


def show_all_books():
    books = store.get_all_books(
    print("\n"))# adding blank line before list of books
    ui.show_books(books)
    print("\n")# adding blank line before list of books

def search_book():
    search_term = ui.ask_question('Enter search term, will match partial authors or titles.')
    print("\n")  # adding blank line before list of books
    matches = store.book_search(search_term)
    print("\n")  # adding blank line before list of books
    ui.show_books(matches)

