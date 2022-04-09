build:
	hugo server -d ./dist/
clean:
	rm -r ./dist/*
post:
	hugo new 'posts/$(POST_NAME).md'
	sed -i 's/Who Are We/$(POST_TITLE)/' content/posts/$(POST_NAME).md
#	sed 's/false/true/' posts/$POST_NAME.md
