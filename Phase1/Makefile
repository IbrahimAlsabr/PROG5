CC=gcc
TARGET=readelf

%.o: %.c
	$(CC) -c $<

readelf: readelf.o elf_reader.o E1_elf_header.o E2_table_section.o E3_content_of_section.o E4_symbole_table.o E5_table_of_reimplantation.o
	$(CC) $^ -o $@ 

clean:
	rm -f *.o

clear:
	rm -f $(TARGET)
