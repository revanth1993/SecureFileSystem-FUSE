#include <errno.h>
#include <stdio.h>
#include <unistd.h>

int main (int argc, char* argv[])
{
 char* path = argv[1];
 int rval;
printf("awd");
 /* Check file existence. */
 rval = access (path, F_OK | R_OK);
 if (rval == 0) 
  printf ("%s exists\n", path);
 else {
  if (errno == ENOENT) 
   printf ("%s does not exist\n", path);
  else if (errno == EACCES) 
   printf ("%s is not accessible\n", path);
  return 0;
 }
}
