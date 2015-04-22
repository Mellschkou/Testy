# Testy
Testy
{
 "cells": [
  {
   "cell_type": "code",
   "execution_count": 1,
   "metadata": {
    "collapsed": false,
    "scrolled": true
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "3\n"
     ]
    }
   ],
   "source": [
    "a = 3\n",
    "\n",
    "print(a) "
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 2,
   "metadata": {
    "collapsed": false
   },
   "outputs": [
    {
     "name": "stdout",
     "output_type": "stream",
     "text": [
      "4\n"
     ]
    }
   ],
   "source": [
    "a = 4 \n",
    "print(a) "
   ]
  },
  {
   "cell_type": "code",
   "execution_count": 3,
   "metadata": {
    "collapsed": false
   },
   "outputs": [
    {
     "data": {
      "text/plain": [
       "<matplotlib.text.Text at 0xa30a940>"
      ]
     },
     "execution_count": 3,
     "metadata": {},
     "output_type": "execute_result"
    },
    {
     "data": {
      "image/png": "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\nAElFTkSuQmCC\n",
      "text/plain": [
       "<matplotlib.figure.Figure at 0x3e345f8>"
      ]
     },
     "metadata": {},
     "output_type": "display_data"
    }
   ],
   "source": [
    "%matplotlib inline\n",
    "import matplotlib.pyplot as plt\n",
    "plt.plot([1,2,3],[7,6,7,])\n",
    "plt.xlabel(\"x\")\n",
    "plt.ylabel(\"y\")\n"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {
    "collapsed": true
   },
   "source": [
    "# This is a title \n",
    "###This is a sub-title \n"
   ]
  },
  {
   "cell_type": "markdown",
   "metadata": {},
   "source": [
    "$$E = m c^2$$\n",
    "\n",
    "The equation $p=h/\\lambda$ is very important"
   ]
  }
 ],
 "metadata": {
  "kernelspec": {
   "display_name": "Python 2",
   "language": "python",
   "name": "python2"
  },
  "language_info": {
   "codemirror_mode": {
    "name": "ipython",
    "version": 2
   },
   "file_extension": ".py",
   "mimetype": "text/x-python",
   "name": "python",
   "nbconvert_exporter": "python",
   "pygments_lexer": "ipython2",
   "version": "2.7.9"
  }
 },
 "nbformat": 4,
 "nbformat_minor": 0
}
