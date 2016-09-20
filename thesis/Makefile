TARGET = main.pdf
OUT_FORMAT = latex
IN_FORMAT = markdown
TEMPLATE = template.tex

.PHONY: all clean

all: $(TARGET)

$(TARGET): *.yaml *.md
	pandoc --template $(TEMPLATE) -f $(IN_FORMAT) -t $(OUT_FORMAT) -s -o $(TARGET) $^

clean:
	-@rm -fR **/*.pdf
