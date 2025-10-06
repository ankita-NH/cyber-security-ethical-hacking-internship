Linux basics -> cheatsheet

whoami -- show current user

pwd -- show current path

ls -la -- list files with permissions and owners

mkdir -p dir

chmod 640 file.txt -- set permissions (owner rw, group r, others none)

chmod go-rw file.txt --remove group+others read/write

chown root:root file --change owner:group (requires sudo)

cat file.txt --display file content
