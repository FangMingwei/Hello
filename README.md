# Hello
PROGRAM hello_world     USE mpi     IMPLICIT NONE      INTEGER  :: ierr, my_rank_all     INTEGER  :: nproc = 4      CALL MPI_INIT(ierr)      CALL MPI_COMM_RANK(MPI_COMM_WORLD, my_rank_all, ierr)     CALL MPI_COMM_SIZE(MPI_COMM_WORLD, nproc, ierr)      WRITE(*,*) 'Hello World!'      CALL MPI_FINALIZE(ierr)      STOP END
